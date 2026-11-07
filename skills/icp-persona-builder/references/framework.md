# Framework completo: ICP & Persona

Detalhamento usado pelo `SKILL.md`. Consultar a seção da etapa em andamento.

## Níveis de evidência

| Nível | Quando usar | Marcação no HTML |
|---|---|---|
| Dado interno | Veio do CRM, pesquisa, entrevista, suporte, uso do produto ou outro dado que o usuário trouxe | `<span class="ev dado">dado interno</span>` |
| Fonte externa | Veio de pesquisa pública, com nome, ano e link conferidos | `<span class="ev fonte">fonte externa <a href="#f1">[1]</a></span>` |
| Suposição | Hipótese de trabalho, sem dado que sustente | `<span class="ev sup">suposição: validar</span>` |

Nunca misturar os níveis sem marcar. Toda suposição relevante entra no plano de validação.

---

## Clientes-semente

O ICP nasce dos melhores clientes atuais.

```
CRITÉRIO DE SUCESSO (definir com o usuário; é do modelo dele)
  Exemplos: retenção acima de 18 meses · expansão de contrato · NPS 9 ou 10
            tempo até o primeiro valor abaixo de 7 dias · pagamento em dia

MELHORES CONTAS (20 a 30)
  Filtro: critério de sucesso + fit com o produto
  Atenção: o maior contrato nem sempre é o cliente ideal

PIORES CONTAS (para os red flags)
  Cancelaram nos primeiros meses · deram prejuízo · exigiram suporte demais
  · compraram por preço e saíram na primeira renovação

PADRÃO
  O que os melhores têm em comum nos 5 componentes?
  O que os piores têm em comum?
```

Sem CRM: pedir de memória os 3 a 5 melhores e os 3 piores clientes, e o que diferencia uns dos outros. Marcar tudo como suposição.

---

## Os 5 componentes

### B2B (nível empresa)

```
1. FIRMOGRAFIA: quem é a empresa
  Setor: [verticais específicas]
  Porte: [funcionários] | Faturamento: [faixa]
  Estágio: [startup / crescimento / consolidada]
  Região: [onde] | Modelo de negócio: [SaaS, indústria, varejo, serviço...]

2. TECNOGRAFIA: o que ela já usa
  Ferramentas: [CRM, ERP, analytics, automação...]
  Solução atual para o problema: [planilha, concorrente, processo manual]
  Maturidade: [adota cedo / adota quando vê outros usando / resiste]
  Por que importa: define integrações, linguagem e objeções técnicas

3. GATILHOS SITUACIONAIS: o que a fez procurar uma solução agora
  - [ex: abriu filial, levantou rodada, contratou head de vendas]
  - [ex: trocou de liderança, trocou de sistema, recebeu autuação]
  - [ex: época do ano em que a compra acontece]
  É o componente mais ignorado e o mais poderoso. A melhor fonte é a pergunta
  de entrevista do gatilho (ver Roteiro de entrevista).

4. SINAIS COMPORTAMENTAIS: como ela se comporta antes e durante a compra
  - [ex: o que faz nos primeiros dias de teste]
  - [ex: quem ela chama para a demonstração]
  - [ex: que conteúdo consome antes de pedir contato]
  Mais confiável que qualquer dado declarado, porque mostra o comportamento
  real da empresa.

5. FIT ECONÔMICO: quanto ela vale
  Ticket: [faixa] | Potencial de expansão: [como cresce dentro da conta]
  LTV estimado: [tempo médio x ticket] | CAC compatível: [quanto dá para gastar]
  Cliente que não se paga não é ICP, mesmo passando em todo o resto.
```

### B2C

Mesma lógica, com os nomes adaptados (usar estes títulos nos cards do HTML):

```
1. PERFIL: idade, renda, região, momento de vida
2. VALORES E ESTILO DE VIDA: o que importa, como se enxerga, aspirações, quem influencia
3. MOMENTOS DE VIDA: o que aconteceu que fez a pessoa procurar agora
   (mudança, filho, promoção, problema de saúde, data do ano)
4. COMPORTAMENTO: onde pesquisa, por impulso ou pesquisa longa, plataformas,
   fidelidade a marca
5. FIT ECONÔMICO: ticket, frequência de compra, recorrência, LTV
```

### Frase-resumo

Duas linhas no máximo, juntando os componentes mais decisivos. Exemplo:
"Indústria de 100 a 500 funcionários no Sul e Sudeste, com time fiscal de 2 a 6 pessoas, que acabou de abrir uma filial e ainda baixa XML na mão."

---

## Scorecard

Ferramenta para vendas decidir em 30 segundos se um lead é o cliente certo. ICP sem scorecard fica só na apresentação.

```
GREEN FLAGS (5 a 8): priorizar
  [critério] · Onde checar: [site / LinkedIn / CRM / consulta de CNPJ / primeira conversa]

RED FLAGS (5 a 8): descartar ou cuidar
  [critério] · Por quê: [dado que justifica, ex: "geram 54% do churn"]

REGRA DE USO
  Ex: 3 ou mais green flags e nenhum red flag: prioridade.
      Um red flag: só segue com motivo claro. Dois ou mais: fora do ICP.
```

Regras:
- Cada critério precisa ser verificável antes ou durante a primeira conversa. "Tem cultura de dados" não serve; "tem analista de dados no LinkedIn" serve.
- Green flags vêm dos melhores clientes; red flags vêm dos piores.
- Cobrir os 5 componentes, principalmente gatilho e fit econômico.
- Quando houver, citar exemplos reais de clientes que se encaixam e que não se encaixam.

---

## Dores e objetivos

```
Dor: [problema específico]
  Categoria: funcional / financeira / processo / social / emocional
  Severidade: [1-10] | Frequência: [diária / semanal / mensal / pontual]
  Contorno atual: [como lida hoje]
  Custo de não resolver: [o que acontece se continuar assim; em horas, dinheiro ou risco]
  Citação: "[frase de cliente]"
```

```
Objetivo principal: [resultado nº 1] | Métrica: [como mede] | Prazo: [esperado]
Objetivos secundários: [2 ou 3]
JTBD: "Quando eu [situação], eu quero [ação], para poder [resultado]."
  Funcional: o que precisa ser feito
  Emocional: como quer se sentir
  Social: como quer ser visto
```

## Objeções

```
PREÇO: "Não temos orçamento" -> [resposta + prova necessária]
TIMING: "Não é o momento de trocar" -> [custo de esperar + facilidade de migração]
CONFIANÇA: "Nunca ouvi falar" -> [prova social + garantia]
INÉRCIA: "A solução atual funciona" -> [custo escondido do jeito atual]
AUTORIDADE: "Preciso de aprovação" -> [conta pronta para levar ao decisor]
TÉCNICA: "Vai integrar com o que já uso?" -> [documentação + caso com a mesma ferramenta]
```

Usar só as que aparecem no caso. A objeção mais frequente nos negócios perdidos vem primeiro.

## Canais

```
| Canal           | Relevância (1-5) | Tipo de conteúdo | Evidência          |
|-----------------|------------------|------------------|--------------------|
| [canal]         | [nota]           | [formato]        | [dado / suposição] |

Ex. de canais: indicação, parceiros, busca no Google, LinkedIn, Instagram,
comunidades, eventos e associações do setor, e-mail, YouTube.
```

---

## Roteiro de entrevista

### Versão curta (20 minutos, a do guia)

5 a 10 clientes-semente. A pergunta principal é a do gatilho:

> **"O que aconteceu na sua empresa que fez você procurar uma solução como a nossa naquele momento?"**

Depois dela, aprofundar com:
1. O que você usava antes? O que não funcionava?
2. Quem mais participou da decisão?
3. O que quase fez você desistir de contratar?
4. Qual foi o primeiro resultado que você percebeu?
5. Se a gente sumisse amanhã, o que você faria?

### Versão completa (30 a 45 minutos)

Meta: 10 a 15 entrevistas. Mix: clientes atuais (5 a 7), clientes que cancelaram (2 a 3), prospects (3 a 5).

```
CONTEXTO (5 min)
1. Me conta sobre seu papel e o seu dia a dia.
2. Quais os maiores desafios na área de [tema]?
3. Como você lida com [problema] hoje?

GATILHO (5 min)
4. O que aconteceu que fez você procurar uma solução naquele momento?

PROBLEMA (10 min)
5. Descreve a última vez que [problema] aconteceu.
6. Qual a parte mais frustrante?
7. Com que frequência isso acontece?
8. O que acontece se não for resolvido?
9. O que você já tentou antes?

SOLUÇÃO (10 min)
10. Que ferramentas você já usou?
11. O que você gosta na solução atual? O que mudaria?
12. Como seria a solução ideal?

COMPRA (10 min)
13. Como você encontrou a sua solução atual?
14. Quem mais participou dessa decisão?
15. O que faria você trocar de fornecedor? O que te seguraria?
16. Quanto você pagaria por [benefício principal]?

FECHAMENTO: Mais alguma coisa? Conhece alguém parecido que toparia conversar?
```

### Síntese pós-entrevistas

```
TEMAS COMUNS: [tema, mencionado por X de N, citações]
GATILHOS: [o que fez cada um procurar, agrupado]
DESCOBERTAS SURPREENDENTES: [o inesperado]
SUPOSIÇÕES CONFIRMADAS: [quais]
SUPOSIÇÕES DERRUBADAS: [quais; é a parte mais valiosa]
AJUSTES NO ICP E NO SCORECARD: [o que muda]
```

### Desenho de pesquisa (survey)

10 a 15 perguntas, 5 a 7 minutos. Usar depois das entrevistas, para validar em quantidade.

- **Triagem** (2 a 3): cargo, porte da empresa, faz [atividade relevante]?
- **Problema** (3 a 4): frequência, severidade (1 a 10), solução atual, satisfação (1 a 10)
- **Solução** (3 a 4): ordem de importância das funcionalidades, motivos para trocar, disposição a pagar
- **Perfil** (2 a 3): setor, orçamento, aceita conversar depois?

Mínimo: 100 respostas para análise quantitativa, 30 para tendência.

---

## Plano de validação

Uma entrada por suposição relevante, da que mais muda decisão para a que menos muda.

```
O QUE VALIDAR: [a suposição, em forma de pergunta]
COMO: [entrevista de 20 min / pesquisa / cruzar CRM com dado público / teste de campanha]
COM QUEM: [perfil e quantidade, ex: "5 gerentes financeiros de clientes atuais"]
PRAZO: [semanas]
SE CONFIRMAR: [o que muda no ICP, no scorecard ou na mensagem]
SE CAIR: [o que fazer no lugar]
PERGUNTAS: [quando for entrevista: 3 a 5 perguntas do roteiro, adaptadas,
            sempre com a pergunta do gatilho]
```

Priorizar o que é barato e rápido de validar (cruzar CRM, consulta de CNPJ) antes do que é caro (pesquisa grande).

## Checklist de qualidade do ICP

- [ ] Baseado em dado (entrevistas, pesquisas, CRM, uso), não só em suposição
- [ ] 10 ou mais clientes reais batem com o perfil
- [ ] Clientes dentro do ICP têm LTV maior e churn menor que os de fora
- [ ] Os clientes do ICP são alcançáveis pelos canais identificados
- [ ] Os 5 componentes estão preenchidos, não só a firmografia
- [ ] Existe scorecard com critérios checáveis em 30 segundos
- [ ] Específico o bastante para guiar decisão, sem excluir o mercado inteiro
- [ ] Compartilhado com marketing, vendas, sucesso do cliente e produto

Revisar: a cada 50 clientes novos, depois de mudança de preço, depois de lançamento relevante, ao entrar em mercado novo e, no mínimo, a cada trimestre.

---

## Persona

### Cartão de persona (campo a campo)

```
PERSONA: [Nome fácil de lembrar, ex: "Analista Ana"] · iniciais para o monograma
Cargo: [título] | Empresa: [tipo e porte] | Idade: [faixa]
Papel na compra: [usa / influencia / decide / pode vetar]

BIO: [2 a 3 frases de comportamento, não só demografia.
      "35 a 45 anos, trabalha remoto, ativa em grupos de WhatsApp do setor"
      diz mais que "35 a 45 anos, mora em SP"]

CITAÇÃO: "[frase que revela o jeito de pensar, não só um fato.
           Fraca: 'preciso de ferramentas melhores'.
           Forte: 'perco 3 horas por semana copiando dado de um sistema para
           o outro e ninguém valoriza isso']"

JTBD PRINCIPAL: "Quando eu [situação], eu quero [ação], para poder [resultado]."

DORES (3)                  GANHOS DESEJADOS (3)
- [dor específica]         - [ganho mensurável]

INSIGHT INESPERADO: [padrão que ninguém esperaria e que muda uma decisão de
                     produto, marketing ou venda. Explicar por que importa.]

NA DECISÃO: [tem orçamento? até quanto? precisa de aprovação de quem?]
INFLUENCIADORES: [quem molda a decisão: chefe, pares, contador, comunidade]
FERRAMENTAS: [3 a 5 que usa]

MENSAGEM: Dizer "[o que ressoa]" | Evitar "[o que afasta]"
Prova que convence: [case, número, depoimento, demonstração]

OBJEÇÃO: "[maior hesitação]" -> "[como responder]"

EVIDÊNCIA E CONFIANÇA
  Confiança: [Alta / Média / Baixa]
  Validado: [o que veio de dado real, com origem]
  Suposição: [o que é hipótese]
  Em aberto: [o que falta pesquisar]
```

### Modo hipótese (proto-persona) e modo validado

| Proto-persona (hipótese)                  | Persona validada                           |
|-------------------------------------------|--------------------------------------------|
| Criada em horas ou dias                   | Criada ao longo de semanas ou meses        |
| Suposição + pesquisa limitada             | Pesquisa extensa                           |
| Serve para alinhar o time rápido          | Serve para guiar produto e mensagem        |
| Muda rápido                               | Estável                                    |
| "Bom o suficiente para começar"           | Alta confiança                             |

Nunca tratar proto-persona como fato. Marcar as suposições e usar a persona para guiar as próximas entrevistas, não para substituir a pesquisa.

### Erros comuns

- ICP só com firmografia ("B2B de 100 a 500 funcionários" é segmentação, sem gatilho nem contexto de compra)
- ICP sem scorecard, que ninguém consegue aplicar no dia a dia
- Demografia sem comportamento ("28 anos, mora em SP" não explica por que ela compraria)
- Tratar suposição como fato
- Criar mais de 4 personas de uma vez (começar com 2 ou 3 e expandir depois de validar)
- Citação inventada que soa como texto de propaganda
- Inventar rótulo ou gíria para o segmento em vez de usar as palavras dos clientes
- Nunca revisar o ICP depois de pronto

### Boas práticas

- Cruzar dado quantitativo (pesquisa, CRM, uso) com qualitativo (entrevista)
- Olhar padrões fora do óbvio: às vezes o segmento mais valioso está nos clientes que fogem da média
- Definir o ICP principal e também segmentos secundários aceitáveis
- O ICP dá foco; não precisa excluir toda oportunidade fora dele
- Compartilhar com a empresa toda, não só com marketing
