# Ideias de projetos: pricing, FP&A e regulação

> 📍 Você está em: [início](../README.md) › [Portfólio](README.md) › **Ideias para pricing, FP&A e regulação**

Três projetos pensados para espelhar as [6 vagas de referência](../carreira/vagas-referencia.md).
Cada um responde a uma pergunta que alguém nessas vagas responde de verdade.

**Regras para todos:**
- Começa com uma **pergunta de negócio**, termina com uma **recomendação**.
- Quando os dados forem simulados, o README diz isso logo no início, e diz por quê.
- Impacto sempre como **business case com hipóteses explícitas**, nunca ROI inventado (ver [análise do post](../carreira/analise-post-portfolio-roi.md)).
- README no modelo [`templates/projeto-README.md`](../templates/projeto-README.md), com versão curta em inglês.

> ⚠️ Os nomes de bases de dados abaixo existiam em 2026, mas sites mudam. Confira o link e a documentação antes de começar.

---

## Projeto 1 · Qual anuidade maximiza o resultado do cartão? (pricing e elasticidade)

**Espelha:** V4 e V5 (Bradesco pricing), em parte V2 (Sicoob).

**Pergunta:** se o banco aumentar a anuidade ou reduzir o cashback, quantos clientes cancelam, e o resultado melhora ou piora? Varia por segmento?

**Por que dados simulados:** a elasticidade real de um banco depende de dados internos de clientes, que não são públicos.
A solução honesta é simular uma base de clientes **com elasticidades que você define**, e mostrar que o seu método as recupera.
Isso, aliás, é como se valida um método antes de usá-lo com dados reais.

**Dados:**
- Simulados: base de clientes com segmento, renda, gasto mensal, anuidade e se cancelou (gerados em Python).
- Reais, para contexto: estatísticas de meios de pagamento e taxas de juros por modalidade do Banco Central (inclui cartão rotativo), e dados de mercado publicados pela Abecs.

**Método, passo a passo:**
1. SQL (DuckDB, gratuito e local) para montar a tabela de rentabilidade por cliente: receita de anuidade + intercâmbio + juros − custo de cashback − perda esperada.
2. Experimento simulado: um grupo recebe aumento de preço, outro não. Estimar o efeito com diferenças em diferenças e com regressão log-log (dois caminhos para a mesma pergunta; comparar).
3. Curva de resultado x preço por segmento.
4. Business case: três cenários (elasticidade otimista, central, pessimista) e recomendação.

**Entregas:** notebook Python, consultas SQL, planilha de cenários, uma página no Power BI e um resumo executivo de 1 página.

**Frase de currículo (exemplo):**
"Estimei a elasticidade da base de clientes de cartão à anuidade por segmento (SQL, Python) e construí business case com três cenários, recomendando reajuste diferenciado por segmento."

---

## Projeto 2 · Reajuste tarifário de uma distribuidora de energia, recalculado (regulação econômica)

**Espelha:** V6 (CPFL).

**Pergunta:** de onde vem cada parte da tarifa de energia de uma distribuidora, e quanto ela mudaria se o custo de capital regulatório ou a inflação fossem diferentes?

**Dados (todos públicos):**
- Portal de dados abertos da ANEEL: tarifas homologadas e componentes tarifários por distribuidora.
- Notas técnicas dos processos tarifários publicadas pela ANEEL.
- Procedimentos de Regulação Tarifária (PRORET), que descrevem a metodologia.
- IPCA e outras séries macro no SGS do Banco Central e no IBGE.

**Conceitos que você vai praticar:**
- **Parcela A:** custos que a distribuidora não controla (compra de energia, transmissão, encargos) e que são repassados.
- **Parcela B:** custos que ela controla (operação, remuneração e depreciação dos investimentos), corrigidos pela inflação menos o **Fator X** no reajuste anual.
- **Reajuste anual x revisão periódica:** o reajuste corrige; a revisão recalcula a Parcela B do zero a cada ciclo.

**Método, passo a passo:**
1. Escolher uma distribuidora e baixar as componentes tarifárias de alguns anos.
2. Reproduzir em Excel o cálculo simplificado do reajuste, citando a nota técnica.
3. Análise de sensibilidade: o que acontece com a tarifa se o custo de capital variar 1 ponto percentual? E se a inflação dobrar?
4. Comparar a composição da tarifa entre 5 distribuidoras (Python ou Power BI).
5. Escrever 2 páginas no formato de **contribuição a consulta pública**: problema, evidência, proposta.

**Entregas:** planilha do cálculo, gráfico de composição da tarifa, texto técnico curto.

**Frase de currículo (exemplo):**
"Reproduzi o cálculo do reajuste tarifário de uma distribuidora a partir das notas técnicas da ANEEL e simulei a sensibilidade da tarifa ao custo de capital regulatório (Excel, Python)."

**Por que este projeto é especial para você:** quase ninguém que estuda dados faz um projeto de regulação.
Em uma vaga com poucos candidatos qualificados, ele te diferencia muito.

---

## Projeto 3 · Orçado x realizado de uma empresa SaaS (FP&A)

**Espelha:** V3 (FP&A SaaS) e V1 (Bluehost).

**Pergunta:** a empresa está batendo o orçamento? Onde está o desvio, e ele vem de preço, de volume de clientes ou de churn?

**Por que dados simulados:** empresas não publicam orçamento interno. Você cria uma SaaS fictícia, com regras de geração documentadas.

**Dados:** 24 meses simulados de uma SaaS fictícia: clientes novos, cancelamentos, plano contratado, preço, custo de aquisição, despesas por centro de custo. Gerar em Python ou Excel. Um arquivo "orçado" e um arquivo "realizado".

**Métricas que você vai calcular:** MRR, ARR, churn, LTV, CAC, LTV/CAC, DRE gerencial mensal.

**Método, passo a passo:**
1. Power Query para juntar orçado e realizado (o tipo de automação que a V1 pede: "automate periodic reporting").
2. Modelo estrela no Power BI e medidas DAX para as métricas.
3. **Análise de desvio preço x volume x mix**: quanto do desvio da receita vem de cada fator.
4. Forecast dos próximos 6 meses em três cenários.
5. Página executiva: 3 conclusões e uma recomendação para a diretoria.

**Entregas:** arquivo Power BI (prints no README), planilha com o modelo, resumo executivo.

**Frase de currículo (exemplo):**
"Construí painel de orçado x realizado de uma SaaS (Power BI, Power Query, DAX), decompondo o desvio de receita em preço, volume e churn, com forecast em três cenários."

---

## Bônus (só se mirar tesouraria) · ALM simplificado

Para a V2: carteira fictícia de crédito e captação, com curva de juros real (DI e Selic no SGS do Banco Central).
Calcular o descasamento de prazos e o impacto de um choque de 1 ponto na taxa sobre a margem. Faça depois da CEA, se for o caminho.

---

## Em que fase do curso cada projeto entra

Dois jeitos de ordenar. Escolha conforme a sua prioridade (ver [diagnóstico, passo 3](../carreira/diagnostico-pricing-fpa.md)).

| Ordem | Se a prioridade é... | Sequência |
|---|---|---|
| **Pela ferramenta** (segue as fases) | Aprender em ordem e montar portfólio junto | Fase 1 (Excel) → Projeto 2 · Fase 2 (Power BI) → Projeto 3 · Fase 3 (Python) → Projeto 1 |
| **Pelo emprego mais rápido** | Ter algo para mostrar em FP&A logo | Projeto 3 primeiro (Excel + Power BI), depois 1 e 2 |

Recomendação: **ordem pela ferramenta**, porque cada projeto usa exatamente o que a fase acabou de ensinar
e o Projeto 2 é feito quase todo em Excel, que é o requisito mais frequente nas vagas.
