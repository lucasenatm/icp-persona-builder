---
name: icp-persona-builder
description: "Constroi ICP (perfil de cliente ideal) e personas de forma integrada, unindo frameworks de firmografia, JTBD, dores, objecoes, canais e evidencia/confianca. Gera como entrega final um arquivo HTML unico com o ICP e as personas prontos pra compartilhar ou imprimir. Use sempre que o usuario pedir pra definir cliente ideal, ICP, buyer persona, perfil de cliente, publico-alvo, segmentacao de clientes, ou pedir pra 'criar uma persona', 'quem e meu cliente ideal', mesmo que nao use essas palavras exatas."
---

# ICP & Persona Builder

Skill de construção de ICP (Ideal Customer Profile) e personas, feita pra funcionar em qualquer negócio B2B ou B2C. Junta num fluxo só o que geralmente fica espalhado em skills separadas de firmografia, JTBD, pesquisa de cliente e persona, e entrega um HTML único no final: o documento de referência que o time todo (marketing, vendas, produto) pode usar.

Entrega final: **um arquivo HTML autocontido** com o ICP completo e de 2 a 4 personas, pronto pra abrir no navegador ou imprimir.

## Como funciona

1. Levantar contexto do negócio (dado interno do usuário)
2. Complementar com pesquisa de mercado externa, onde faltar dado interno
3. Definir o que é validado e o que ainda é hipótese
4. Construir o ICP
5. Construir as personas
6. Validar
7. Gerar o HTML

Ler `references/framework.md` pra estrutura completa de cada etapa (roteiro de entrevista, desenho de survey, e o detalhamento campo a campo do ICP e da persona). Usar `assets/template.html` como base de layout e CSS pro HTML final.

## Passo 1 — Levantar contexto

Antes de qualquer outra pergunta, pedir pro usuário todos os dados de clientes que ele já tiver disponível: pesquisas (survey), planilhas exportadas do CRM, relatórios de suporte/atendimento, estudos de mercado, transcrições de entrevista, dados de analytics/uso, dados de churn. Se ele mandar arquivo (CSV, Excel, PDF, texto), ler e analisar diretamente antes de seguir — não pedir pra ele resumir manualmente o que já está no arquivo.

Isso vem antes de qualquer suposição: quanto mais dado real entrar aqui, menos a etapa 3 e 4 vão depender de hipótese.

Depois, perguntar (ou usar o que já está disponível na conversa/projeto):

- Produto/serviço e o problema que resolve
- Mercado: B2B ou B2C
- Modelo de venda: self-serve, venda assistida, enterprise
- Estágio do negócio: pré-lançamento, early, growth, maduro
- Geografia
- Nome da empresa/marca e, se tiver, cor principal (só pra estilizar o HTML — se não tiver, usar uma paleta neutra)

Se o usuário tiver um one-pager, guia interno ou material de referência próprio sobre como construir ICP, pedir esse material e priorizar a estrutura dele sobre o framework genérico abaixo.

## Passo 2 — Complementar com pesquisa de mercado

Depois de esgotar o dado interno do usuário, olhar o que ainda ficou em aberto no ICP (tamanho de mercado, comportamento do setor, benchmark de preço, dado demográfico, tendência do segmento) e buscar dado público que preencha essa lacuna: estudos setoriais, relatórios de institutos, dados de associações de classe, benchmarks de mercado, matérias e pesquisas publicadas. Usar busca na internet pra isso.

Regras pra essa pesquisa:
- Priorizar fonte primária (instituto de pesquisa, órgão do setor, relatório oficial) sobre blog secundário
- Toda informação trazida de fonte externa entra no documento com citação: nome da fonte, ano, e link
- Se não achar dado público confiável pra alguma lacuna, não forçar — deixar como suposição mesmo, marcada como tal
- Pesquisa de mercado complementa o dado interno, nunca substitui. Se o usuário já tem dado próprio sobre algo, esse dado vale mais que uma média de mercado genérica

## Passo 3 — Classificar o que é validado e o que é hipótese

Cada afirmação relevante do ICP e da persona cai em um destes três níveis:

- **Validado (dado interno)**: veio de pesquisa, entrevista, CRM, analytics ou outro dado que o próprio usuário trouxe
- **Validado (fonte externa)**: veio de pesquisa de mercado pública, com citação de fonte e link
- **Suposição**: hipótese de trabalho, sem dado que sustente ainda, marcada com `[SUPOSIÇÃO — VALIDAR]`

Marcar cada seção principal do ICP e da persona com o nível correspondente, e nunca apresentar suposição como se fosse dado validado — nem interno nem externo.

## Passo 4 — Construir o ICP

Preencher no formato B2B ou B2C conforme o mercado (ver `references/framework.md#icp` pro detalhamento completo):

**B2B (nível empresa):** firmografia (setor, tamanho, geografia, modelo de negócio), tecnografia (stack, maturidade tecnológica), gatilhos situacionais (eventos que criam urgência de compra), critérios de qualificação (obrigatório / desejável / desqualificante).

**B2C (nível indivíduo):** demografia, psicografia (valores, identidade, aspirações), traços comportamentais (plataformas, consumo de conteúdo, comportamento de compra).

**Comum aos dois:**
- JTBD (funcional, emocional, social)
- Dores e objetivos, com severidade, frequência e custo de não resolver
- Objeções mais comuns e como responder
- Mapeamento de canais onde esse cliente está

## Passo 5 — Construir as personas

Criar de 2 a 4 personas dentro do ICP. Cada persona precisa ter (ver `references/framework.md#persona` pro campo a campo):

- Nome memorável (aliteração ajuda, ex: "Analista Ana") + cargo/papel
- Bio comportamental (não só demografia: o que faz no dia a dia, como decide, onde busca informação)
- Citação representativa (real, de entrevista, ou marcada como hipótese)
- JTBD principal
- Top 3 dores + top 3 ganhos/resultados desejados
- Um insight inesperado (padrão contraintuitivo que muda decisão de produto ou marketing)
- Autoridade de decisão e quem influencia essa pessoa
- Mensagem: o que falar / o que evitar falar
- Maior objeção + resposta
- Evidência e confiança: o que é validado, o que é suposição, o que falta pesquisar

Personas precisam ser distintas entre si. Se duas personas compartilham a mesma dor principal e o mesmo JTBD, provavelmente são a mesma persona — fundir.

## Passo 6 — Validar

Antes de gerar o HTML, checar:

- [ ] Baseado em dado real (interno ou de fonte externa citada) ou claramente marcado como suposição
- [ ] Toda fonte externa usada tem nome, ano e link registrados
- [ ] Critérios específicos o bastante pra guiar decisão, sem ser tão estreito que exclua o mercado
- [ ] Personas distintas entre si
- [ ] Seção de evidência e confiança preenchida
- [ ] Linguagem acionável pra marketing, vendas e produto usarem direto

## Passo 7 — Gerar o HTML

Ler `assets/template.html` e usar como referência de estrutura e CSS (autocontido, responsivo, sóbrio, sem dependência de recursos externos, funciona offline). Adaptar o conteúdo:

- Cabeçalho com nome da empresa/produto e data de criação
- Seção do ICP (B2B ou B2C conforme o caso)
- Uma seção por persona, repetindo o cartão de acordo com quantas personas foram criadas (2 a 4)
- Seção final de **Fontes e Referências**, listando toda fonte externa citada (nome, ano, link) usada em qualquer parte do documento — se não houve pesquisa externa, omitir essa seção
- Rodapé com a nota geral de evidência/confiança e data sugerida pra próxima revisão (a cada trimestre, ou após mudança relevante de produto, preço ou mercado)

Salvar o arquivo com nome `icp-persona-[nome-da-empresa].html` na pasta que o usuário indicar (perguntar se não tiver ficado claro onde salvar).
