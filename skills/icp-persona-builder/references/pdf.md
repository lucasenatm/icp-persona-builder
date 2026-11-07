# Gerar o PDF

O PDF sai do `assets/pdf-template.html`, preenchido com o mesmo conteúdo do HTML e convertido pelo próprio navegador (Chrome, Edge, Chromium ou Brave) em modo headless. Não precisa instalar nada.

## 1. Montar o HTML do PDF

Salvar o template preenchido como `icp-persona-[empresa]-pdf.html`, na mesma pasta do HTML final. É um arquivo intermediário: depois que o PDF estiver pronto e conferido, apagar.

## 2. Achar o navegador

Testar nesta ordem e usar o primeiro que existir:

**Windows**
```
C:\Program Files\Google\Chrome\Application\chrome.exe
C:\Program Files (x86)\Google\Chrome\Application\chrome.exe
%LOCALAPPDATA%\Google\Chrome\Application\chrome.exe
C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe
C:\Program Files\Microsoft\Edge\Application\msedge.exe
```
O Edge vem instalado em todo Windows.

**macOS**
```
/Applications/Google Chrome.app/Contents/MacOS/Google Chrome
/Applications/Microsoft Edge.app/Contents/MacOS/Microsoft Edge
/Applications/Chromium.app/Contents/MacOS/Chromium
/Applications/Brave Browser.app/Contents/MacOS/Brave Browser
```

**Linux**
```
google-chrome  google-chrome-stable  chromium  chromium-browser  microsoft-edge
```

## 3. Conferir se nenhuma página estourou

Cada página tem altura fixa de A4. O script do template marca no `<html>` quais páginas passaram do limite:

```
"<navegador>" --headless=new --disable-gpu --virtual-time-budget=15000 --dump-dom "file:///<caminho absoluto>/icp-persona-[empresa]-pdf.html"
```

Na saída, olhar a tag `<html ... data-overflow="" data-pages="10">`:

- `data-overflow` vazio: tudo coube.
- `data-overflow="7,9"`: as páginas 7 e 9 estouraram. Mover o excesso para uma página de continuação logo depois dela (mesmo cabeçalho, "(continuação)" no `.pg-sec`) ou enxugar o texto. Rodar de novo até vir vazio.

O `--virtual-time-budget` dá tempo para a fonte Sora carregar antes da medição. Sem internet, o documento usa a fonte do sistema, e a medição já considera isso.

## 4. Converter

```
"<navegador>" --headless=new --disable-gpu --no-pdf-header-footer --virtual-time-budget=15000 --print-to-pdf="<caminho absoluto>/icp-persona-[empresa].pdf" "file:///<caminho absoluto>/icp-persona-[empresa]-pdf.html"
```

Detalhes:
- O caminho do arquivo vira URL: no Windows, `file:///C:/Users/...` com barras normais; espaço vira `%20`.
- O template já define `@page` com A4 e margem zero. Não tirar: sem ele, o navegador transforma as páginas em imagem e o PDF passa de 50 MB.

## 5. Conferir o resultado

- O arquivo existe e tem menos de 5 MB (o normal fica entre 1 e 2 MB).
- O número de páginas bate com o `data-pages`.
- Se der para abrir ou renderizar o PDF, olhar a capa e uma página de persona.

## Se não houver navegador compatível

**Com Node instalado:** usar o Puppeteer numa pasta temporária.

```js
// npm install puppeteer  (numa pasta temporária)
const puppeteer = require('puppeteer');
(async () => {
  const browser = await puppeteer.launch({ headless: 'new' });
  const page = await browser.newPage();
  await page.goto('file:///<caminho absoluto>/icp-persona-[empresa]-pdf.html', { waitUntil: 'networkidle0' });
  await page.evaluate(() => document.fonts.ready);
  console.log(await page.evaluate(() => document.documentElement.dataset.overflow));
  await page.pdf({ path: '<caminho absoluto>/icp-persona-[empresa].pdf', printBackground: true, preferCSSPageSize: true });
  await browser.close();
})();
```

**Sem Node:** abrir o `icp-persona-[empresa]-pdf.html` no navegador, apertar Ctrl+P (Cmd+P no Mac) e escolher: destino "Salvar como PDF", margens "Nenhuma", "Gráficos de plano de fundo" ligado. Explicar isso ao usuário e manter o arquivo intermediário até ele salvar.
