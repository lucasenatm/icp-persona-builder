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

### Dentro do Claude Code

Abra o Claude Code no terminal e rode os dois comandos, um de cada vez:

```
/plugin marketplace add lucasenatm/icp-persona-builder
```

```
/plugin install icp-persona-builder@icp-persona-builder
```

No segundo, escolha **Install for you** para ter a skill em qualquer pasta. Se aparecer `Run /reload-plugins to apply`, rode `/reload-plugins` (ou feche e abra o Claude Code).

### Pelo terminal do sistema

Sem abrir o Claude Code:

```
claude plugin marketplace add lucasenatm/icp-persona-builder
claude plugin install icp-persona-builder@icp-persona-builder
```

A skill aparece na próxima vez que você abrir o Claude Code.

### VS Code e app desktop

No painel do Claude Code no VS Code, digite `/plugins`, adicione `lucasenatm/icp-persona-builder` na aba **Marketplaces** e instale o plugin na aba **Plugins**.

O terminal, o VS Code e o app desktop leem as mesmas configurações: instalou em um, vale nos outros.

### Conferir se deu certo

Digite `/` e procure por `icp-persona-builder`. A skill aparece como `/icp-persona-builder:icp-persona-builder`.

### O que precisa ter

- **Claude Code**
- **Chrome, Edge, Chromium ou Brave**, para gerar o PDF. O Edge já vem em todo Windows. A skill usa o navegador em modo invisível e não instala nada.
- **Internet**, para a pesquisa de mercado e para a fonte do documento

---

## Como usar

Digite `/icp-persona-builder:icp-persona-builder` ou só peça: "define meu cliente ideal", "cria uma persona para o meu produto", "quem é o meu ICP".

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

Plugins de fora da loja oficial do Claude Code não se atualizam sozinhos. Para pegar a versão nova:

- **Dentro do Claude Code:** rode `/plugin`, vá na aba **Marketplaces**, selecione `icp-persona-builder` e escolha **Update marketplace**. Na mesma tela, **Enable auto-update** deixa a atualização automática daqui para frente.
- **Pelo terminal do sistema:** `claude plugin update icp-persona-builder@icp-persona-builder`

Depois, rode `/reload-plugins` ou abra uma sessão nova. As mudanças de cada versão estão em [Releases](https://github.com/lucasenatm/icp-persona-builder/releases).

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
