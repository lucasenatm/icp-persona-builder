# icp-persona-builder

Plugin para Claude Code que monta o ICP (perfil de cliente ideal) e as personas do seu negócio a partir dos seus dados reais, e entrega tudo em dois arquivos: um HTML interativo para navegar e um PDF diagramado para mandar e imprimir.

Segue o método do guia gratuito **[Como montar um ICP B2B de verdade](https://lucasena.com/lp-icp-b2b)**: partir dos seus melhores clientes, preencher os 5 componentes e fechar com um scorecard que vendas aplica em 30 segundos.

Feito por [lucasena.](https://lucasena.com)

---

## O que você ganha

A skill lê os dados que você tiver (CRM, pesquisas, entrevistas, suporte, churn), encontra o padrão dos seus melhores clientes e completa as lacunas com pesquisa de mercado citada. No final, entrega um HTML e um PDF com:

- **Frase-resumo do ICP** e um medidor de quanto do documento é dado e quanto é suposição
- **Os 5 componentes**: firmografia, tecnografia, gatilhos situacionais, sinais comportamentais e fit econômico
- **Scorecard** de green flags e red flags, cada um checável no site, no LinkedIn ou na primeira conversa
- **JTBD, dores com custo, objeções com resposta e canais**
- **2 a 4 personas** com citação, insight inesperado, papel na decisão e o que dizer e evitar
- **Plano de validação**: o que ainda é suposição, como validar, com quem e com quais perguntas
- **Fontes** de toda pesquisa externa

Cada afirmação vem marcada como dado interno, fonte externa ou suposição. Nada de chute apresentado como fato.

Antes de gerar os arquivos, a skill mostra um rascunho para você ajustar. O HTML funciona no celular e no modo escuro. O PDF é diagramado página por página em A4, com capa, resumo, sumário e uma página por persona. Os dois seguem a identidade visual da lucasena.

Funciona para qualquer negócio, B2B ou B2C. Sem dado nenhum, ela também roda: o resultado vira um ponto de partida, com o plano de validação como parte principal.

---

## Instalação

### Copie, cole e pronto

Copie o texto abaixo, cole no Claude Code e aperte enter. Funciona no app do Claude, no VS Code e no terminal.

```
Instala para mim a skill de ICP e personas do Lucas Sena.

1. Rode este comando: claude plugin install icp-persona-builder --marketplace lucasenatm/icp-persona-builder
2. Se o comando "claude" não existir nesta máquina, baixe https://github.com/lucasenatm/icp-persona-builder/archive/refs/heads/master.zip, descompacte e copie a pasta skills/icp-persona-builder para ~/.claude/skills/icp-persona-builder
3. No final, me diga em uma frase se deu certo e o que eu faço para começar a usar.
```

Se o Claude pedir permissão para rodar o comando, é só aceitar. Depois, abra uma conversa nova e peça: **"monta o ICP da minha empresa"**.

### Sem Claude Code (site ou app do Claude)

No claude.ai ou no app do Claude, vá em **Customize > Plugins**, clique em **Add > Add marketplace**, cole `lucasenatm/icp-persona-builder` e instale o `icp-persona-builder` que aparece na lista.

Precisa de plano pago e da opção **Code execution and file creation** ligada em **Settings > Capabilities**. O plugin fica salvo na sua conta e também aparece no Claude Code. Se ali não der para gerar o PDF direto, a skill entrega um arquivo para você salvar como PDF pelo navegador (Ctrl+P).

<details>
<summary><b>Prefere digitar os comandos?</b></summary>

Dentro do Claude Code:

```
/plugin install icp-persona-builder --marketplace lucasenatm/icp-persona-builder
```

Escolha **Install for you** e, se aparecer `Run /reload-plugins to apply`, rode `/reload-plugins`. Em versões antigas do Claude Code, use dois comandos: `/plugin marketplace add lucasenatm/icp-persona-builder` e depois `/plugin install icp-persona-builder@icp-persona-builder`.

Pelo terminal do sistema, sem abrir o Claude Code:

```
claude plugin install icp-persona-builder --marketplace lucasenatm/icp-persona-builder
```

</details>

### O que precisa ter

- **Claude Code** ou **plano pago do Claude** (para usar pelo site ou pelo app)
- **Chrome, Edge, Chromium ou Brave** para gerar o PDF. O Edge já vem em todo Windows, e a skill não instala nada.
- **Internet** para a pesquisa de mercado

---

## Como usar

Abra uma conversa nova e só peça: "monta o ICP da minha empresa", "define meu cliente ideal", "cria uma persona para o meu produto". Se preferir o comando, digite `/` e procure por `icp-persona-builder`.

O fluxo:

1. Você manda os dados que tiver
2. A skill resume o que encontrou e pergunta só o que faltou, incluindo onde você quer crescer
3. Encontra os clientes-semente: os melhores e os piores da base
4. Pesquisa o mercado para cobrir lacunas, com fonte e link
5. Monta o ICP com os 5 componentes e o scorecard
6. Monta as personas
7. Mostra o rascunho para você ajustar
8. Gera o HTML com o plano de validação
9. Gera o PDF diagramado

---

## Atualizar

A skill não se atualiza sozinha. Para pegar a versão mais nova, cole no Claude Code:

```
Atualiza a skill icp-persona-builder para a versão mais nova. Rode: claude plugin update icp-persona-builder@icp-persona-builder. Se ela estiver instalada como pasta em ~/.claude/skills/icp-persona-builder, baixe de novo https://github.com/lucasenatm/icp-persona-builder/archive/refs/heads/master.zip e troque a pasta pela nova.
```

Depois, abra uma conversa nova. Pelo site ou app do Claude, a atualização fica em **Customize > Plugins**. As mudanças de cada versão estão em [Releases](https://github.com/lucasenatm/icp-persona-builder/releases).

---

## Estrutura do plugin

```
skills/
  icp-persona-builder/
    SKILL.md              fluxo completo (9 passos)
    references/
      framework.md        5 componentes, scorecard, roteiro de entrevista, persona e plano de validação
      pdf.md              como converter o PDF com o navegador e conferir as páginas
    assets/
      template.html       modelo do HTML interativo
      pdf-template.html   modelo do PDF em páginas A4
      lucasena-*.png      logo do crédito no rodapé (versão escura e clara)
```

---

## Licença

MIT
