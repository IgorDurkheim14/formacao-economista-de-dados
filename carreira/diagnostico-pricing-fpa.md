# Diagnóstico: o que o mestrado já cobre e o que falta

> 📍 [início](../README.md) › [Carreira](README.md) › **Diagnóstico pricing, FP&A e regulação**

Baseado na [matriz de requisitos das 6 vagas](vagas-referencia.md) de 21/11/2026.
É um diagnóstico de "médico": primeiro entender o quadro, depois escolher o tratamento.

> ⚠️ Eu não conheço ainda o seu currículo nem as disciplinas exatas do seu mestrado.
> Onde escrevi "provavelmente", é hipótese. Corrija o que não bater.

---

## Passo 1 · O que o mestrado já entrega (e como cada vaga chama isso)

O ponto mais importante deste documento: **você já tem muita coisa, mas com outro nome.**
O recrutador procura a palavra do mercado; o seu currículo provavelmente usa a palavra da academia.

| O que você aprendeu no mestrado | Como a vaga chama | Onde aparece |
|---|---|---|
| Regressão log-log, elasticidade-preço da demanda | "Análise de elasticidade e comportamento de clientes" | V5 |
| Econometria, inferência causal (diferenças em diferenças, variáveis instrumentais) | "Avaliar impacto de mudanças de preço, campanhas e benefícios" | V4, V5 |
| Séries temporais, projeção | "Forecast", "projeções", "cenários" | V1, V2, V3, V4, V5 |
| Microeconomia: monopólio natural, regulação por preço-teto | "Equilíbrio econômico-financeiro da concessão", "revisão tarifária" | V6 |
| Macroeconomia: juros, Selic, curva de juros | "Sensibilidade a taxas de juros", "custo de funding" | V2 |
| Escrever dissertação, argumentar com evidência | "Contribuições técnicas a consultas públicas", "relatórios executivos" | V6, V3 |
| Dissertação com dados de satélite e PIB municipal | "Projetos com modelagem avançada", "nowcasting" | V4, V5 |

### Exemplo concreto

A mesma coisa escrita de dois jeitos:

- **Jeito acadêmico:** "Estimação de modelo log-log com efeitos fixos para a demanda."
- **Jeito de pricing:** "Estimei quanto a demanda cai a cada 1% de aumento de preço, para decidir o preço que maximiza a receita."

O conteúdo é idêntico. Só o segundo passa na triagem de uma vaga de pricing.

> ✋ **Está acompanhando?** Se esta tabela fizer sentido, você já percebe que parte do problema não é
> "falta de conhecimento", é **tradução**. Essa é a parte rápida de resolver.

---

## Passo 2 · O que falta, separado por tempo de solução

Pensei em três prazos, porque eles pedem estratégias diferentes.

### 🟢 Rápido (semanas, depende só de você)

| Lacuna | Por que importa | Prazo realista |
|---|---|---|
| Currículo e LinkedIn traduzidos para a linguagem do mercado | É a primeira porta; hoje ela parece fechada | 1–2 semanas |
| Vocabulário de negócio: DRE, budget, forecast, margem, spread, custo de funding, MRR, churn, Parcela A/B | Entrevista e currículo pedem essas palavras | 2–4 semanas de leitura |
| Excel para finanças: tabela dinâmica, PROCX, SOMASES, tabela de dados, gerenciador de cenários | Aparece em 5 de 6 vagas | 4–8 semanas |
| Power BI básico | 4 de 6 vagas | 4–6 semanas (já está na Fase 2) |

### 🟡 Médio (3 a 6 meses de estudo constante)

| Lacuna | Comentário |
|---|---|
| SQL até nível intermediário (JOIN, GROUP BY, funções de janela) | Obrigatório para pricing em banco (V4, V5) |
| Python com pandas e statsmodels | Você provavelmente já sabe a econometria; falta a ferramenta. Se usou Stata ou R no mestrado, a transição é mais rápida |
| Matemática financeira aplicada: VPL, TIR, juros compostos, duration | Base de pricing de crédito (V2) e tarifa (V6) |
| 2 ou 3 projetos de portfólio que imitam as vagas | Ver [ideias de projetos](../portfolio/ideias-pricing-fpa-regulacao.md) |
| **CEA (ANBIMA)** | Só se você mirar tesouraria de banco ou cooperativa (V2). É uma certificação de especialista em investimentos, com prova. Confira regras, custo e conteúdo no site da ANBIMA antes de decidir |

### 🔴 Demorado (anos, não depende só de estudo)

| Lacuna | Por que é difícil |
|---|---|
| **Experiência no domínio** (cartões, tesouraria, processos tarifários, FP&A) | Pedida em 5 de 6 vagas. Se aprende trabalhando |
| **Senioridade** ("Sr", "III", "Specialist") | Quatro das seis vagas são sênior ou acima. Para quem está entrando na área, são alvo de 2 a 3 anos, não de agora |
| Databricks e dados em escala de banco | Dá para treinar na versão gratuita, mas o uso real vem no emprego |

---

## Passo 3 · Como contornar o que é demorado

Não há atalho para experiência, mas há **mais de um caminho**. Eles podem ser combinados.

| Caminho | Como funciona | Prós | Contras |
|---|---|---|---|
| **A · Mirar um degrau abaixo** | Candidatar-se a "Analista Pleno" ou "Júnior" de pricing, FP&A ou regulação, em vez de "Sr" ou "Specialist" | Maior chance de passar na triagem; a experiência vem em 1–2 anos | Salário inicial menor |
| **B · Portfólio que imita o domínio** | Projetos com dados públicos que resolvem o problema da vaga (pricing de cartão, revisão tarifária, budget SaaS) | Mostra que você entende o negócio, não só a ferramenta | Não substitui experiência; ajuda a ser chamado para conversar |
| **C · Contar o mestrado como experiência** | Se teve bolsa, projeto de pesquisa ou consultoria, listar como experiência profissional com entregas | Preenche o "buraco" no currículo | Precisa ser descrito com resultado, não com disciplinas |
| **D · Portas laterais** | Consultorias regulatórias e econômicas, cooperativas e bancos médios, fintechs, agências reguladoras (concurso) | Exigem menos tempo de casa e valorizam o mestrado | Menor visibilidade; exige pesquisa ativa |
| **E · Indicação (networking)** | Conversar com quem trabalha em pricing ou regulação e pedir indicação | A indicação costuma pular parte da triagem automática | Leva tempo para construir relacionamento |

### Minha recomendação (com o raciocínio)

1. **Família principal: pricing / rentabilidade.** É onde econometria, elasticidade e causalidade valem mais,
   e onde o título de mestre pesa. É também a família mais próxima do objetivo do curso
   (Economista de Dados / Cientista de Dados Quantitativo).
2. **Família de apoio: regulação econômica.** O seu perfil de economista com escrita técnica encaixa muito bem,
   e há poucos candidatos com esse perfil. A barreira é a experiência tarifária, que um projeto de portfólio ajuda a reduzir.
3. **FP&A como porta de entrada mais rápida.** A V3 (SaaS) nem pede anos de experiência. Excel + Power BI + um
   projeto de orçado x realizado já te deixam competitivo para vagas de analista. Serve como primeiro emprego na área,
   enquanto você constrói o resto.
4. **Adiar a CEA**, a menos que surjam várias vagas de tesouraria que você queira muito.

**Outra forma de pensar:** se a sua urgência for empregar-se rápido, inverta a ordem e ponha FP&A em primeiro.
Se a urgência for o cargo certo a longo prazo, mantenha pricing em primeiro. As duas são defensáveis.

> ✋ **Pergunta para você:** qual pesa mais agora, conseguir o primeiro emprego em dados logo ou mirar
> direto pricing? A resposta muda a ordem da trilha.

---

## Passo 4 · Onde a trilha atual do curso deve mudar

A trilha de hoje é: Fase 1 SQL, Excel e estatística → Fase 2 Power BI → Fase 3 Python e econometria → Fase 4 ML, causal e séries → Fase 5 deploy.
Para estas vagas, ela está boa na base, mas tem **uma lacuna** (finanças de negócio) e **uma ênfase desalinhada** (ML cedo demais para o que as vagas pedem).

Proposta de ajuste (não aplicada ainda nas pastas; aguardando o seu ok):

| Mudança | Por quê |
|---|---|
| **Fase 1: Excel antes de SQL**, com um bloco de Excel financeiro (cenários, sensibilidade, tabela de dados) | Excel aparece em 5 de 6 vagas; SQL em 2 |
| **Novo módulo na Fase 1: "Finanças para dados"** (matemática financeira, DRE, budget e forecast, rentabilidade, pricing básico) | É o vocabulário que falta e aparece em quase todas as vagas |
| **Fase 2: projeto de portfólio = orçado x realizado de uma SaaS** | Espelha V1 e V3 |
| **Fase 3: trazer a elasticidade para cá** (econometria em Python aplicada a preço) | Espelha V4 e V5, e usa o que você já sabe |
| **Fase 4: priorizar inferência causal e séries temporais; ML vira opcional** | Nenhuma das 6 vagas pede ML como requisito; só aparece como diferencial |
| **Fase 5: sem mudança**, mas deploy só se sobrar tempo | Nenhuma vaga pede deploy |
| **Em paralelo a tudo:** currículo, LinkedIn e networking a partir da semana 1 | Não espere terminar o curso para se candidatar |
