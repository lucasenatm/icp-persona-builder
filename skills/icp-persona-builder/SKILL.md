---
name: icp-persona-builder
description: "Constrói o ICP (perfil de cliente ideal) e as personas de um negócio a partir dos dados reais dele, seguindo os 5 componentes (firmografia, tecnografia, gatilhos situacionais, sinais comportamentais e fit econômico), com scorecard de green flags e red flags para vendas, personas, plano de validação e marcação clara do que é dado e do que é suposição. Entrega um HTML interativo e um PDF diagramado em A4, os dois com visual pronto para compartilhar. Use sempre que o usuário pedir para definir cliente ideal, ICP, buyer persona, perfil de cliente, público-alvo, segmentação de clientes ou critérios de qualificação de leads, ou pedir para 'criar uma persona' ou 'descobrir quem é meu cliente ideal', mesmo sem usar essas palavras exatas."
---

# ICP & Persona Builder

Constrói o ICP e as personas de qualquer negócio B2B ou B2C e entrega dois arquivos que marketing, vendas e produto usam no dia a dia: um HTML interativo, para navegar na tela, e um PDF diagramado página por página, para mandar e imprimir.

O método é o do guia "Como montar um ICP B2B de verdade" ([lucasena.com/lp-icp-b2b](https://lucasena.com/lp-icp-b2b)): partir dos melhores clientes atuais, preencher os 5 componentes e fechar com um scorecard que o time consegue aplicar em 30 segundos.

**O que os dois arquivos trazem:**
- frase-resumo do ICP e um medidor de quanto do documento é dado e quanto é suposição
- os 5 componentes do ICP
- scorecard de green flags e red flags
- JTBD, dores com custo, objeções com resposta e canais
- de 2 a 4 personas
- plano para validar as suposições
- fontes de toda pesquisa externa

## Princípios

- **Dado antes de suposição.** Toda afirmação importante recebe um nível de evidência: dado interno, fonte externa ou suposição. Nunca apresentar suposição como fato.
- **ICP serve para decidir.** Quem priorizar, quem descartar, o que falar. Se uma informação não ajuda a decidir nada, cortar.
- **Conversa curta.** Ler os dados primeiro e perguntar só o que eles não responderam. Juntar as perguntas numa mensagem só.
- **Vocabulário do cliente.** Usar as palavras que aparecem nas entrevistas, no suporte e nas pesquisas. Nunca inventar gíria, apelido ou rótulo de segmento.

## Fluxo

1. Pedir os dados
2. Ler, resumir e perguntar o que falta
3. Encontrar os clientes-semente
4. Pesquisar o mercado para cobrir lacunas
5. Construir o ICP e o scorecard
6. Construir as personas
7. Mostrar o rascunho e ajustar
8. Montar o plano de validação e gerar o HTML
9. Gerar o PDF

Ler `references/framework.md` para o detalhamento de cada parte (campos dos 5 componentes, scorecard, roteiro de entrevista, cartão de persona, plano de validação). Usar `assets/template.html` como base obrigatória do HTML final e `assets/pdf-template.html` como base do PDF; o passo a passo da conversão está em `references/pdf.md`.

## Passo 1: pedir os dados

Antes de qualquer outra pergunta, pedir todos os dados de clientes que o usuário já tiver:

- export do CRM (clientes, negócios ganhos e perdidos, receita ou plano, data de cancelamento)
- pesquisas e formulários respondidos por clientes
- conversas de atendimento, suporte, WhatsApp ou e-mail
- transcrições ou anotações de entrevistas e reuniões
- dados de uso do produto, NPS, churn
- estudos de mercado que ele já tenha

Se ele mandar arquivo (CSV, planilha, PDF, texto), ler e analisar direto. Nunca pedir para ele resumir o que já está no arquivo.

**Se não houver dado nenhum:** avisar logo no início que o resultado vai ser um ponto de partida, com personas em modo hipótese, e que o plano de validação será a parte mais importante do documento. Seguir com o passo 2 e, no passo 3, usar a versão sem CRM.

## Passo 2: ler, resumir e perguntar o que falta

Depois de ler os dados, mostrar um resumo curto do que eles revelam (5 a 8 tópicos: quem compra e fica, quem sai e por quê, quando compram, o que mais dói, como a venda acontece, onde estão os clientes). Isso mostra que os arquivos foram lidos e deixa o usuário corrigir alguma leitura errada.

Em seguida, numa mensagem só, perguntar apenas o que os dados não responderam:

- produto ou serviço e o problema que resolve
- B2B ou B2C
- modelo de venda: compra sozinho pelo site, venda consultiva, venda complexa com várias pessoas decidindo
- estágio do negócio: pré-lançamento, primeiros clientes, crescimento, consolidado
- geografia
- **foco: existe algum segmento que a empresa quer priorizar ou abandonar?** Sempre perguntar. O ICP descreve onde a empresa quer crescer, e a base atual nem sempre é isso. Quando o foco for diferente da base, usar a base como evidência e o foco como alvo, e deixar claro no documento o que é cada um.
- nome da empresa (vai na capa do documento; o visual é fixo, não precisa perguntar cor)
- onde salvar o arquivo final (perguntar já aqui para não interromper no fim)

Se o usuário tiver um material próprio sobre ICP (guia, modelo, one-pager), pedir e priorizar a estrutura dele.

## Passo 3: encontrar os clientes-semente

O ICP nasce dos melhores clientes atuais. A média da base esconde o padrão.

1. **Definir o critério de sucesso com o usuário.** Exemplos: retenção acima de 18 meses, expansão de contrato, NPS alto, tempo curto até o primeiro valor, pagamento em dia. O critério é do modelo dele; não existe certo universal. Se os dados já sugerem um critério, propor e pedir confirmação.
2. **Filtrar as 20 a 30 melhores contas** pela combinação desse critério com fit com o produto. O maior contrato nem sempre é o cliente ideal.
3. **Olhar também os piores clientes** (cancelaram rápido, deram prejuízo, exigiram suporte demais). É deles que saem os red flags do scorecard.
4. Procurar o que os melhores têm em comum e o que os piores têm em comum, nos 5 componentes.

**Sem CRM:** pedir para o usuário citar de memória os 3 a 5 melhores clientes e os 3 piores, e o que diferencia uns dos outros. Tudo o que vier daqui é suposição.

## Passo 4: pesquisar o mercado para cobrir lacunas

Com o dado interno esgotado, buscar na internet dado público para o que ficou em aberto: tamanho do segmento, comportamento do setor, benchmarks, regulação, tendências.

- Priorizar fonte primária: instituto de pesquisa, órgão do governo, associação de classe, relatório oficial.
- Conferir o número na própria fonte (abrir a página ou o PDF). Não citar número que só apareceu num resumo de busca.
- Registrar nome da fonte, ano e link de tudo o que entrar no documento.
- Se não achar dado confiável, não forçar: deixar como suposição e colocar no plano de validação.
- Pesquisa de mercado complementa o dado interno, nunca substitui. Dado próprio do usuário vale mais que média de mercado.

## Passo 5: construir o ICP e o scorecard

**Os 5 componentes** (detalhe em `references/framework.md#os-5-componentes`):

1. **Firmografia:** quem é a empresa (setor, porte, faturamento, estágio, região, modelo de negócio)
2. **Tecnografia:** o que ela já usa (ferramentas, solução atual para o problema, maturidade)
3. **Gatilhos situacionais:** o que aconteceu que a fez procurar uma solução agora. É o componente mais ignorado e o mais poderoso.
4. **Sinais comportamentais:** como ela se comporta antes e durante a compra (o que faz no teste, quem chama para a conversa, o que consome)
5. **Fit econômico:** quanto ela vale (ticket, potencial de expansão, LTV, CAC compatível). Cliente que não se paga não é ICP, mesmo passando em todo o resto.

No B2C, os componentes mudam de nome e mantêm a lógica (perfil, valores e estilo de vida, momentos de vida, comportamento, fit econômico). Ver `references/framework.md#b2c`.

**Junto dos componentes:**
- frase-resumo do ICP, que caiba em duas linhas
- JTBD funcional, emocional e social
- 3 a 5 dores, com severidade de 1 a 10, frequência e custo de não resolver
- 3 a 6 objeções, cada uma com a resposta
- canais com relevância de 1 a 5

**Scorecard** (detalhe em `references/framework.md#scorecard`): 5 a 8 green flags e 5 a 8 red flags, cada um verificável por vendas em 30 segundos (site, LinkedIn, CRM, consulta de CNPJ, primeira conversa), com uma regra de uso simples. Exemplo: "3 ou mais green flags e nenhum red flag: prioridade". Os red flags vêm dos piores clientes do passo 3.

## Passo 6: construir as personas

De 2 a 4 personas dentro do ICP, normalmente cobrindo quem usa, quem influencia e quem decide. Começar com 2 ou 3; a quarta só se for claramente diferente. Cada persona tem (campo a campo em `references/framework.md#persona`):

- nome fácil de lembrar (ex: "Analista Ana") e cargo
- bio de comportamento: o que faz no dia a dia, como decide, onde busca informação
- citação que revela o jeito de pensar (real, de entrevista, ou marcada como suposição)
- JTBD principal
- 3 dores e 3 ganhos desejados
- um insight inesperado, que muda alguma decisão de produto, marketing ou venda
- papel na decisão e quem a influencia
- mensagem: o que dizer e o que evitar
- maior objeção e a resposta
- confiança (alta, média ou baixa), o que é validado, o que é suposição e o que falta pesquisar

Se duas personas têm a mesma dor principal e o mesmo JTBD, são a mesma persona: fundir.

## Passo 7: mostrar o rascunho e ajustar

Antes de gerar o HTML, mostrar na conversa um rascunho compacto:

- a frase-resumo do ICP
- os 5 componentes, uma linha cada
- os 3 principais green flags e red flags
- cada persona em duas linhas (nome, papel, JTBD, insight)

Perguntar: "Faz sentido? Quer mudar alguma coisa antes de eu montar o documento?" Ajustar com base na resposta. Corrigir uma persona aqui custa uma mensagem; depois do HTML pronto, custa refazer o documento.

## Passo 8: montar o plano de validação e gerar o HTML

**Plano de validação** (detalhe em `references/framework.md#plano-de-validação`): para cada suposição importante, em ordem de impacto, dizer o que validar, como (entrevista, pesquisa, cruzamento de CRM, teste de campanha), com quem e quantas pessoas, em quanto tempo, e o que muda no ICP se confirmar ou se cair. Quando o método for entrevista, incluir as perguntas, adaptadas ao caso, sempre com a pergunta do gatilho: "O que aconteceu na sua empresa que fez você procurar uma solução como a nossa naquele momento?"

**Checklist antes de gerar:**

- [ ] Cada afirmação importante tem nível de evidência
- [ ] Toda fonte externa tem nome, ano e link, e o número foi conferido na fonte
- [ ] Os 5 componentes estão preenchidos (com suposição marcada onde faltou dado)
- [ ] O scorecard tem critérios que vendas consegue checar em 30 segundos
- [ ] Critérios específicos o bastante para guiar decisão, sem excluir o mercado inteiro
- [ ] Personas diferentes entre si
- [ ] Toda suposição relevante está no plano de validação
- [ ] O texto está claro para quem não participou da conversa

**Gerar o HTML:**

- Ler `assets/template.html` e seguir as instruções do comentário no topo. Manter o `<head>` (CSS e fonte), o `<script>` do fim, a estrutura e os componentes visuais; trocar todo o conteúdo. O visual segue a identidade da lucasena. (fonte Sora, coral, preto e off-white) e não muda de cliente para cliente.
- Escrever títulos normalmente, com maiúsculas onde couber: o CSS já deixa títulos, rótulos e chips em minúsculas.
- Manter o rodapé com o crédito "feito por lucasena." exatamente como está no template.
- Marcar a evidência com as classes `ev dado`, `ev fonte` e `ev sup`. O medidor da capa se calcula sozinho a partir delas.
- Apagar a seção de fontes se não houve pesquisa externa.
- Salvar como `icp-persona-[nome-da-empresa].html` no local combinado no passo 2.

## Passo 9: gerar o PDF

O PDF é uma peça própria, diagramada em páginas A4. Não é o HTML impresso. Seguir `references/pdf.md`:

1. Preencher `assets/pdf-template.html` com o mesmo conteúdo do HTML, reorganizado nas páginas: capa, resumo (3 descobertas mais importantes e sumário), componentes, scorecard, motivação e dores, objeções e canais, uma página por persona, plano de validação e fontes. Manter o `<head>` e o `<script>` como estão.
2. Salvar como `icp-persona-[nome-da-empresa]-pdf.html`, ao lado do HTML.
3. Conferir com o navegador headless se alguma página estourou e, se estourou, criar página de continuação ou enxugar o texto.
4. Converter para `icp-persona-[nome-da-empresa].pdf` com o mesmo navegador.
5. Conferir tamanho e número de páginas e apagar o `-pdf.html` intermediário.

Se não houver navegador compatível nem Node, seguir o plano B de `references/pdf.md` (Ctrl+P com as opções certas) e avisar o usuário.

**Mensagem final para o usuário:** onde os dois arquivos foram salvos, as 3 descobertas mais importantes e o primeiro passo do plano de validação.

## Como escrever o documento

- Frases curtas, em linguagem que marketing, vendas e produto entendem sem explicação.
- Números com fonte ou com origem interna clara ("38% dos clientes do CRM").
- Sem jargão vazio ("solução 360", "transformação digital") e sem citação que soe como texto de propaganda.
- Sem travessão (—): usar vírgula, ponto ou dois-pontos.
