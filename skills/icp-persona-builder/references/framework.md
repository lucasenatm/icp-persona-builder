# Framework completo — ICP & Persona

Detalhamento campo a campo usado pelo `SKILL.md`. Consultar as seções conforme a etapa em andamento.

## ICP

### B2B (nível empresa)

```
FIRMOGRAFIA
  Setor: [verticais específicas]
  Tamanho (funcionários): [faixa] | Tamanho (receita): [faixa]
  Estágio: [startup/scaleup/enterprise/público]
  Geografia: [regiões] | Modelo de negócio: [SaaS/e-commerce/agência/etc.]

TECNOGRAFIA
  Stack: [ferramentas que usam] | Solução atual: [pro problema em questão]
  Maturidade tecnológica: [early adopter/mainstream/laggard]

GATILHOS SITUACIONAIS (eventos que criam urgência de compra)
  - [ex: "acabou de crescer além de X funcionários"]
  - [ex: "contrato atual vencendo", "mudança de gestão"]

CRITÉRIOS DE QUALIFICAÇÃO
  Obrigatório: [ex: "time fiscal de 3+ pessoas"]
  Desejável: [ex: "já usa integração via API"]
  Desqualificante: [ex: "menos de 10 funcionários", "sem orçamento definido"]
```

### B2C (nível indivíduo)

```
DEMOGRAFIA
  Idade: [faixa] | Renda: [faixa] | Localização: [região]
  Momento de vida: [estudante/início de carreira/pai-mãe/aposentado]

PSICOGRAFIA
  Valores: [o que importa pra essa pessoa]
  Identidade: [como se enxerga]
  Aspirações: [o que busca alcançar]
  Influências: [quem molda as decisões dela]

TRAÇOS COMPORTAMENTAIS
  Plataformas: [redes, busca, fóruns]
  Conteúdo: [podcasts, newsletters, YouTube]
  Comportamento de compra: [por impulso vs. pesquisa profunda]
  Fidelidade à marca: [troca fácil vs. fiel]
```

### Dores e objetivos

```
Dor: [problema específico]
  Severidade: [1-10] | Frequência: [diária/semanal/mensal]
  Contorno atual: [como lida hoje]
  Custo de não resolver: [o que acontece se continuar sem solução]
  Impacto emocional: [frustração/ansiedade/constrangimento]
  Citação: "[frase representativa do cliente]"
```

Categorias de dor: funcional (tarefa difícil/lenta), financeira (custa caro), processo (fluxo quebrado), social (fica mal na frente do chefe/pares), emocional (estresse/sobrecarga).

```
Objetivo principal: [#1 resultado] | Métrica: [como mede] | Prazo: [esperado]
Objetivos secundários: [2-3 outros resultados]
Resultado dos sonhos: [se tudo desse certo]
JTBD: "Quando eu [situação], eu quero [ação], pra poder [resultado]."
```

### Objeções

```
PREÇO: "Não temos orçamento" -> [resposta + prova necessária]
TIMING: "Não é o momento de trocar" -> [custo de esperar + facilidade de migração]
CONFIANÇA: "Nunca ouvi falar" -> [prova social + garantia]
INÉRCIA: "A solução atual funciona" -> [custo escondido do status quo]
AUTORIDADE: "Preciso de aprovação" -> [business case pronto]
TÉCNICA: "Vai integrar com o que já uso?" -> [documentação + suporte]
```

### Mapeamento de canais

```
| Canal          | Relevância (1-5) | Tipo de conteúdo | Custo       |
|-----------------|------------------|------------------|-------------|
| Busca (Google)  | [nota]           | SEO/ads          | grátis/pago |
| LinkedIn        | [nota]           | posts/ads        | grátis/pago |
| Comunidades     | [nota]           | discussão        | grátis      |
| E-mail          | [nota]           | nutrição/vendas  | pago        |
| Eventos/webinar | [nota]           | palestra/patroc. | pago        |
| YouTube         | [nota]           | tutoriais        | grátis/pago |

TOP 3 CANAIS: [canal + por quê + tática]
CONTEÚDO CONSUMIDO: newsletters, comunidades, influenciadores e eventos específicos
```

### Roteiro de entrevista de cliente

Meta: 10-15 entrevistas. Mix: clientes atuais (5-7), churn (2-3), prospects (3-5). Ligações de 30-45 min.

```
CONTEXTO (5 min)
1. Me conta sobre seu papel e o dia a dia.
2. Quais os maiores desafios na área de [tema relevante]?
3. Como você lida com [problema] hoje?

PROBLEMA (10 min)
4. Descreve a última vez que [problema] aconteceu.
5. Qual a parte mais frustrante?
6. Com que frequência isso acontece?
7. O que acontece se não for resolvido?
8. O que você já tentou antes?

SOLUÇÃO (10 min)
9. Que ferramentas você já usou?
10. O que você gosta na solução atual?
11. O que você mudaria?
12. Como seria a solução ideal?

COMPRA (10 min)
13. Como você encontrou sua solução atual?
14. Quem mais participou dessa decisão?
15. O que faria você trocar de fornecedor?
16. O que te seguraria de trocar?
17. Quanto você pagaria por [benefício-chave]?

FECHAMENTO: Mais alguma coisa? Conhece alguém parecido que toparia conversar?
```

### Síntese pós-entrevistas

```
TEMAS COMUNS: [tema, mencionado por X/n, citações-chave]
DESCOBERTAS SURPREENDENTES: [insights inesperados]
SUPOSIÇÕES VALIDADAS: [confirmadas]
SUPOSIÇÕES INVALIDADAS: [derrubadas — crítico]
AJUSTES NO ICP: [mudanças a partir do que foi descoberto]
```

### Desenho de survey

10-15 perguntas, 5-7 minutos. Usar depois das entrevistas pra validação quantitativa.

- **Triagem** (2-3): cargo, tamanho da empresa, faz [atividade relevante]?
- **Problema** (3-4): frequência, severidade (1-10), solução atual, satisfação (1-10)
- **Solução** (3-4): ranking de funcionalidades, gatilhos de troca, disposição a pagar
- **Demografia** (2-3): setor, orçamento, aberto a follow-up?

Mínimo: 100 respostas pra análise quantitativa, 30 pra insights direcionais.

### Checklist de validação do ICP

- [ ] Baseado em dado (entrevistas, surveys, analytics), não só suposição
- [ ] 10+ clientes/prospects reais batem com o perfil
- [ ] Clientes dentro do ICP têm LTV maior e churn menor
- [ ] Clientes do ICP são alcançáveis pelos canais identificados
- [ ] Específico o bastante pra guiar decisão, sem estreitar demais o mercado
- [ ] Documentado e compartilhado com times de marketing, vendas e produto

Revisar: a cada 50 clientes novos, após mudança de preço, após lançamento de feature relevante, após entrada em novo mercado, no mínimo trimestralmente.

---

## Persona

### Cartão de persona (campo a campo)

```
PERSONA: [Nome memorável, ex: "Analista Ana"]
Cargo: [título] | Empresa: [tipo/porte] | Idade: [faixa]

BIO: [2-3 frases: vida profissional, desafios, aspirações — comportamental,
      não só demográfico. "35-45 anos, trabalha remoto, ativa em grupos de
      WhatsApp do setor" diz mais que "35-45 anos, mora em SP"]

CITAÇÃO: "[frase real ou representativa que revela mentalidade, não só fato.
           Fraco: 'preciso de ferramentas melhores'.
           Forte: 'perco 3 horas por semana copiando dado de um sistema pro
           outro e ninguém valoriza isso']"

JTBD PRINCIPAL: "Quando eu [situação], eu quero [ação], pra poder [resultado]."

DORES (top 3)              GANHOS DESEJADOS (top 3)
- [dor 1, específica]      - [ganho 1, mensurável]
- [dor 2]                  - [ganho 2]
- [dor 3]                  - [ganho 3]

INSIGHT INESPERADO: [padrão contraintuitivo — algo que ninguém esperaria e que
                     muda uma decisão de produto ou marketing. Explicar por
                     que importa.]

AUTORIDADE DE DECISÃO: [tem orçamento? até quanto? precisa de aprovação de
                        quem?]
INFLUENCIADORES: [quem molda a decisão dela — chefe, pares, analistas,
                  comunidade, conteúdo que consome]
CRENÇAS E ATITUDES: [o que afeta a disposição de adotar algo novo, ex:
                     "desconfia de ferramenta que promete automação mas
                     exige um dev pra configurar"]

FERRAMENTAS: [3-5 que usa]  CANAIS DE CONFIANÇA: [3-5]

MENSAGEM: Dizer "[o que ressoa com ela]" | Evitar "[o que afasta]"
Benefício-chave: [a #1 coisa que ela valoriza]
Prova necessária: [tipo de evidência que convence — case, dado, depoimento]

OBJEÇÃO: "[maior hesitação]" -> Resposta: "[como endereçar]"

EVIDÊNCIA E CONFIANÇA
  Confiança geral: [Alta/Média/Baixa] — [justificativa]
  Validado: [o que veio de dado real, com fonte]
  Suposição: [o que é hipótese, marcado [SUPOSIÇÃO — VALIDAR]]
  Perguntas em aberto: [o que falta pesquisar pra fechar a lacuna]
```

### Quando usar modo hipótese (proto-persona) vs. modo validado

| Proto-persona (hipótese)                     | Persona validada                          |
|-----------------------------------------------|--------------------------------------------|
| Criada em horas/dias                          | Criada ao longo de semanas/meses           |
| Baseada em suposição + pesquisa limitada      | Baseada em pesquisa extensa                |
| Serve pra alinhar o time rapidamente          | Serve pra guiar decisão de design/messaging|
| Evolui rápido                                 | Estável ao longo do tempo                  |
| "Bom o suficiente pra começar"                | Alta confiança                             |

Nunca tratar proto-persona como fato. Marcar toda suposição com `[SUPOSIÇÃO — VALIDAR]` e usar a persona pra guiar as próximas entrevistas, não pra substituir a pesquisa.

### Erros comuns a evitar

- Demografia sem comportamento ("28 anos, mora em SP" não explica por que ela compraria)
- Tratar suposição como fato validado
- Criar mais de 4 personas de uma vez (gera paralisia — começar com 1-2 e expandir depois de validar)
- Inventar citação que soa como copy de marketing em vez de fala real
- Nunca revisar a persona depois de criada

### Boas práticas gerais

- Cruzar dado quantitativo (survey, analytics) com qualitativo (entrevista)
- Entrevistar 10+ clientes/prospects de alto valor pra identificar padrão
- Prestar atenção em padrão demográfico não óbvio (outliers às vezes são o segmento mais valioso)
- Definir o ICP ideal e também segmentos secundários aceitáveis
- Revisar o ICP e as personas trimestralmente, ou antes disso se o produto, preço ou mercado mudar
- Compartilhar com toda a organização, não só marketing
- O ICP deve dar foco, não excluir toda oportunidade fora dele
