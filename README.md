# icp-persona-builder

Plugin para Claude Code que monta o ICP (perfil de cliente ideal) e as personas do seu negócio a partir dos seus dados reais, e entrega tudo em dois arquivos: um HTML interativo para navegar e um PDF diagramado para mandar e imprimir.

Segue o método do guia gratuito **[Como montar um ICP B2B de verdade](https://lucasena.com/lp-icp-b2b)**: partir dos seus melhores clientes, preencher os 5 componentes e fechar com um scorecard que vendas aplica em 30 segundos.

Feito por [lucasena.](https://lucasena.com)

---

## O que você ganha

**`/icp-persona-builder`** lê os dados que você tiver (CRM, pesquisas, entrevistas, suporte, churn), encontra o padrão dos seus melhores clientes e completa as lacunas com pesquisa de mercado citada. No final, entrega um HTML e um PDF com:

- **Frase-resumo do ICP** e um medidor de quanto do documento é dado e quanto é suposição
- **Os 5 componentes**: firmografia, tecnografia, gatilhos situacionais, sinais comportamentais e fit econômico
- **Scorecard** de green flags e red flags, cada um checável no site, no LinkedIn ou na primeira conversa
- **JTBD, dores com custo, objeções com resposta e canais**
- **2 a 4 personas** com citação, insight inesperado, papel na decisão e o que dizer e evitar
- **Plano de validação**: o que ainda é suposição, como validar, com quem e com quais perguntas
- **Fontes** de toda pesquisa externa

Cada afirmação vem marcada como dado interno, fonte externa ou suposição. Nada de chute apresentado como fato.

Antes de gerar os arquivos, a skill mostra um rascunho para você ajustar. O HTML funciona no celular e no modo escuro. O PDF é diagramado página por página em A4, com capa, resumo, sumário e uma página por persona. Os dois seguem a identidade visual da lucasena.

Para gerar o PDF, a skill usa o Chrome ou o Edge que já estão no seu computador. Não precisa instalar nada.

Funciona para qualquer negócio, B2B ou B2C. Sem dado nenhum, ela também roda: o resultado vira um ponto de partida, com o plano de validação como parte principal.

---

## Instalação

**Mais fácil:** cole este prompt no Claude Code com qualquer pasta aberta.

```
Instala para mim o plugin https://github.com/lucasenatm/icp-persona-builder adicionando as entradas necessárias no ~/.claude/settings.json
```

**Manual:** adicione ao `~/.claude/settings.json`:

```json
"enabledPlugins": {
  "icp-persona-builder@icp-persona-builder": true
},
"extraKnownMarketplaces": {
  "icp-persona-builder": {
    "source": {
      "source": "github",
      "repo": "lucasenatm/icp-persona-builder"
    }
  }
}
```

---

## Como usar

Chame com `/icp-persona-builder` ou peça naturalmente: "define meu cliente ideal", "cria uma persona para o meu produto", "quem é o meu ICP".

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
