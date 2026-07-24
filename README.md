# icp-persona-builder

Plugin pra Claude Code que constrói ICP (perfil de cliente ideal) e personas de forma integrada — junta num fluxo só o que geralmente fica espalhado em skills separadas de firmografia, JTBD, pesquisa de cliente e persona.

Feito por [lucasena.](https://lucasena.com)

---

## O que você ganha

**`/icp-persona-builder`** — constrói o ICP completo (B2B ou B2C) e de 2 a 4 personas distintas, usando dado interno do usuário (pesquisas, CRM, entrevistas) complementado por pesquisa de mercado externa quando falta dado. Classifica cada afirmação como validado (dado interno), validado (fonte externa) ou suposição — nunca mistura os três sem marcar. Entrega final: um **arquivo HTML autocontido**, responsivo e sóbrio, pronto pra abrir no navegador ou imprimir, com seção de fontes e nota de confiança.

Funciona pra qualquer negócio, B2B ou B2C.

---

## Instalação

**Mais fácil:** cole esse prompt no Claude Code com qualquer pasta aberta.

```
Instala pra mim o plugin https://github.com/lucasenatm/icp-persona-builder adicionando as entradas necessárias no ~/.claude/settings.json
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

## Estrutura do plugin

```
skills/
  icp-persona-builder/
    SKILL.md              — fluxo completo (7 passos)
    references/
      framework.md         — estrutura detalhada de ICP e persona, campo a campo
    assets/
      template.html        — layout e CSS base do HTML final
```

## Como usar

Chame com `/icp-persona-builder` ou peça naturalmente: "define meu cliente ideal", "cria uma persona pro meu produto", "quem é meu ICP". A skill pede os dados que você já tiver (pesquisas, CRM, entrevistas), complementa com pesquisa de mercado onde faltar, e gera o HTML final.

---

## Licença

MIT
