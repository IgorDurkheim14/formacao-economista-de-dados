# Guia de estudo: onde aprender, praticar, certificar e o que publicar

> 📍 Você está em: [início](../README.md) › [Recursos](README.md) › **Guia de estudo**

Este guia funciona **sem o Claude**: para cada fase, ele diz de onde tirar o conteúdo, onde praticar,
qual certificado vale a pena e qual projeto de portfólio fazer.

> ⚠️ Preços, gratuidade e regras de certificado mudam com frequência. Confira no site antes de se inscrever.

---

## Como pensar sobre conteúdo, certificado e portfólio

Três coisas diferentes, com pesos diferentes na hora da contratação:

| | O que prova | Peso no processo seletivo |
|---|---|---|
| **Curso / conteúdo** | Que você estudou | Baixo sozinho |
| **Certificado** | Que alguém verificou que você estudou | Médio. Ajuda a passar no filtro do RH e do LinkedIn |
| **Projeto de portfólio** | Que você **resolve problemas** | **Alto.** É o que se discute na entrevista |

**Regra prática:** para cada curso, termine com um projeto seu. Certificado só nos que o mercado reconhece (marcados com ⭐).

### Três caminhos possíveis (escolha um, ou misture)

| Caminho | Como é | Prós | Contras |
|---|---|---|---|
| **A · 100% gratuito** | Kaggle Learn, Microsoft Learn, Fundação Bradesco, ENAP, livros online | Custo zero | Você monta a sequência sozinho (este guia faz isso) |
| **B · Uma plataforma paga** | DataCamp, Alura ou Data Science Academy (assinatura) | Trilha pronta, exercícios no navegador, certificados | Custo mensal; certificado tem pouco peso fora da plataforma |
| **C · Certificações oficiais** | Google Data Analytics, Microsoft PL-300 | Reconhecidas por recrutadores no Brasil e fora | Pagas (PL-300 é prova paga; Coursera tem auxílio financeiro) |

**Recomendação para o seu perfil:** caminho **A** como base + **2 certificados ⭐** (Google Data Analytics na Fase 1 e PL-300 na Fase 2). Para as Fases 3 e 4, o mestrado em economia já cumpre o papel de "certificado"; aí o que pesa são os projetos.

---

## Fase 1 · SQL, Excel e estatística

### SQL
| Tipo | Material | Gratuito? | Certificado? |
|---|---|---|---|
| Aprender | [SQLBolt](https://sqlbolt.com) (interativo, curto) | Sim | Não |
| Aprender | [Kaggle Learn: Intro to SQL e Advanced SQL](https://www.kaggle.com/learn) | Sim | Sim (de conclusão) |
| Aprender | [Mode SQL Tutorial](https://mode.com/sql-tutorial) | Sim | Não |
| Praticar | [HackerRank SQL](https://www.hackerrank.com/domains/sql) e [LeetCode SQL 50](https://leetcode.com/studyplan/top-sql-50/) | Sim | HackerRank tem teste de habilidade com certificado |
| Praticar com dados BR | [Base dos Dados](https://basedosdados.org) (SQL no BigQuery com dados públicos brasileiros) | Sim (cota gratuita) | Não |

### Excel
| Tipo | Material | Gratuito? | Certificado? |
|---|---|---|---|
| Aprender | [Fundação Bradesco · Escola Virtual](https://www.ev.org.br) (Excel básico a avançado) | Sim | Sim |
| Aprender | Canal Hashtag Treinamentos (YouTube) | Sim | Não |
| Aprender | [Escola Virtual de Governo (ENAP)](https://www.escolavirtual.gov.br) (Excel e análise de dados) | Sim | Sim (bom para vagas de governo) |

### Estatística aplicada
| Tipo | Material | Gratuito? |
|---|---|---|
| Revisar com intuição | Canal **StatQuest** (YouTube, inglês, muito didático) | Sim |
| Livro | *Estatística Prática para Cientistas de Dados* (Bruce & Bruce): a ponte entre a estatística que você já sabe e o mercado | Pago |
| Livro | [OpenIntro Statistics](https://www.openintro.org/book/os/) | Sim |

### ⭐ Certificado da fase
**Google Data Analytics Professional Certificate** (Coursera). Cobre SQL, planilhas, visualização e um estudo de caso. Muito conhecido por recrutadores, inclusive fora do Brasil. Coursera oferece **auxílio financeiro** (pedido no próprio curso).

### 🎯 Projeto de portfólio da fase
**"Emprego formal no Brasil: onde e em que setores cresce?"**
- Dados: CAGED/RAIS na Base dos Dados (SQL no BigQuery)
- O que mostrar: consultas SQL com `JOIN`, `GROUP BY`, funções de janela; um resumo em Excel; uma interpretação estatística (o crescimento é diferente entre regiões, ou é ruído?)
- Onde salvar: `01-fundamentos/01-sql/projeto/`

---

## Fase 2 · Power BI, DAX e storytelling

| Tipo | Material | Gratuito? | Certificado? |
|---|---|---|---|
| Aprender | [Microsoft Learn: trilha da certificação PL-300](https://learn.microsoft.com/pt-br/credentials/certifications/data-analyst-associate/) | Sim | O curso não; a prova sim |
| Aprender DAX | [SQLBI](https://www.sqlbi.com) (curso introdutório de DAX gratuito; [DAX Guide](https://dax.guide)) | Sim | Não |
| Praticar | Desafios mensais de painéis: **Onyx Data DataDNA**, **Maven Analytics challenges**, **Workout Wednesday Power BI** | Sim | Não, mas geram projeto pronto |
| Storytelling | Livro *Storytelling com Dados* (Cole Nussbaumer Knaflic) | Pago | — |

### ⭐ Certificado da fase
**Microsoft PL-300: Power BI Data Analyst Associate.** É a certificação de BI mais pedida em vagas no Brasil. A prova é paga; a Microsoft às vezes distribui vouchers de desconto em eventos/desafios do Microsoft Learn.

### 🎯 Projeto de portfólio da fase
**"Painel da inflação brasileira (IPCA)"**: por grupo de produtos, por região metropolitana, acumulado em 12 meses vs meta.
- Dados: IBGE/SIDRA e Banco Central (SGS)
- O que mostrar: modelo estrela, medidas DAX (acumulado 12m, variação ano contra ano), uma página de conclusões escrita para gestor
- Publicar: "Publicar na Web" do Power BI (se o painel não tiver dado sensível) + prints e o `.pbix` no GitHub

---

## Fase 3 · Python, pandas e econometria

| Tipo | Material | Gratuito? | Certificado? |
|---|---|---|---|
| Base | **Curso em Vídeo**, Python (Gustavo Guanabara, YouTube, português) | Sim | Sim (no site) |
| Base | [Kaggle Learn: Python, Pandas, Data Visualization](https://www.kaggle.com/learn) | Sim | Sim (de conclusão) |
| Livro | [Python para Análise de Dados](https://wesmckinney.com/book/) (Wes McKinney, criador do pandas; versão online em inglês) | Sim | — |
| ⭐ **Para economista** | [QuantEcon](https://quantecon.org/lectures/): *Python Programming for Economics and Finance* | Sim | Não |
| Econometria | Documentação e exemplos do [statsmodels](https://www.statsmodels.org) | Sim | — |

> 💡 O QuantEcon foi feito por economistas para economistas. É o material que mais conversa com o seu mestrado.

### 🎯 Projeto de portfólio da fase
**"Retorno da educação no Brasil"** (equação minceriana com PNAD Contínua), ou uma reescrita em Python da sua dissertação.
- O que mostrar: limpeza com pandas, gráficos com seaborn, regressão com statsmodels e erros robustos, conclusão para leigos
- Diferencial: explicar **por que** a regressão não é causal e o que seria preciso para ser

---

## Fase 4 · Machine Learning, inferência causal e séries temporais

| Tema | Material | Gratuito? | Certificado? |
|---|---|---|---|
| ML | [Kaggle Learn: Intro e Intermediate Machine Learning](https://www.kaggle.com/learn) | Sim | Sim |
| ML | **Machine Learning Specialization** (Andrew Ng, Coursera) | Auxílio financeiro | Sim |
| ML (livro) | [ISLP: An Introduction to Statistical Learning with Python](https://www.statlearning.com) | Sim (PDF oficial) | — |
| ⭐ Causal | [Causal Inference for the Brave and True](https://matheusfacure.github.io/python-causality-handbook/) (Matheus Facure, brasileiro, em Python) | Sim | — |
| Causal | [Causal Inference: The Mixtape](https://mixtape.scunning.com) (Scott Cunningham) | Sim (online) | — |
| Causal | [The Effect](https://theeffectbook.net) (Nick Huntington-Klein) | Sim (online) | — |
| Séries | [Forecasting: Principles and Practice](https://otexts.com/fpppy/) (Hyndman, versão em Python) | Sim | — |
| Praticar | Competições do [Kaggle](https://www.kaggle.com/competitions) (comece pelas "Getting Started") | Sim | Medalhas no perfil |

### 🎯 Projetos de portfólio da fase (escolha 2)
1. **Previsão de inadimplência** (ML): base pública de crédito do Kaggle; validação correta, métricas explicadas em termos de dinheiro.
2. **Avaliação de impacto** (causal): diferenças em diferenças sobre uma política pública brasileira com dados municipais. **Este é o projeto que mais te diferencia** de outros candidatos.
3. **Previsão do IPCA** (séries): SARIMA e um modelo de ML comparados com as expectativas do boletim Focus.

---

## Fase 5 · Git, nuvem e deploy

| Tema | Material | Gratuito? | Certificado? |
|---|---|---|---|
| Git | [GitHub Skills](https://skills.github.com) (exercícios dentro do próprio GitHub) | Sim | Não |
| Git | [Pro Git](https://git-scm.com/book/pt-br/v2) (livro oficial, em português) | Sim | — |
| Nuvem | [Google Cloud Skills Boost](https://www.cloudskillsboost.google) (BigQuery) | Parcial | Selos (badges) |
| Deploy | [Documentação do Streamlit](https://docs.streamlit.io) + Streamlit Community Cloud | Sim | — |

### 🎯 Projeto de portfólio da fase
**App em Streamlit** que mostra um projeto da Fase 4 (ex.: previsão do IPCA com gráfico interativo), publicado com link aberto.

---

## Plataformas brasileiras gratuitas com certificado (bons complementos)
- **Fundação Bradesco · Escola Virtual**: Excel, Power BI introdutório, lógica de programação
- **Escola Virtual de Governo (ENAP)**: análise de dados, ciência de dados, Power BI; valoriza o currículo para governo
- **DIO (Digital Innovation One)**: bootcamps gratuitos patrocinados por empresas, com certificado
- **Curso em Vídeo**: Python e lógica

---

## Rotina de cada curso dentro deste repositório
1. Registre o curso na tabela de [`recursos/README.md`](README.md).
2. Anotações com suas palavras em `<fase>/<módulo>/anotacoes/`.
3. Exercícios em `<fase>/<módulo>/exercicios/`.
4. Ao terminar: salve o PDF do certificado em [`carreira/certificados/`](../carreira/certificados/README.md) e adicione no LinkedIn.
5. Faça o projeto do módulo e, se ficar bom, leve para [`portfolio/`](../portfolio/README.md).
6. Publique no LinkedIn (modelo em [`carreira/curriculo-e-linkedin.md`](../carreira/curriculo-e-linkedin.md)).
