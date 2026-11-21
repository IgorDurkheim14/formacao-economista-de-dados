# Análise crítica: post "portfólio de BI precisa mostrar ROI"

> 📍 [início](../README.md) › [Carreira](README.md) › **Análise do post sobre ROI**

**Contexto:** post de LinkedIn (Gabriel Vaz) dizendo que portfólio de Analista de BI Sênior precisa mostrar
dívida técnica resolvida, ROI em número e automação com agentes de IA. Lido em 21/11/2026.

Como ler qualquer conselho de carreira: separe **o princípio** (geralmente bom) da **embalagem** (geralmente exagerada para engajar).

---

## O que vale (guarde isto)

| Ideia do post | Por que é boa | Como aplicar no seu caso |
|---|---|---|
| Portfólio precisa partir de um **problema concreto** | Recrutador e gestor querem saber se você resolve problemas, não se sabe desenhar gráficos | Todo projeto começa com uma pergunta de negócio ("qual anuidade maximiza a receita do cartão?") |
| Mostrar **antes e depois com número** | Número é o que se lembra e se discute na entrevista | Use números verdadeiros ou estimados com hipótese explícita |
| **Documentar o porquê** de cada decisão | Mostra raciocínio, que é o que você quer vender ("médico, não operador") | Seção "por que escolhi este método e não outro" em cada README |
| Mostrar **código, prints e fluxo** | Prova que foi você quem fez | GitHub com README, gráfico principal e código organizado |
| Dashboard bonito sozinho não basta | É verdade: visual sem conclusão não ajuda quem decide | Todo painel termina com 3 conclusões e uma recomendação |

A estrutura **problema → solução → impacto em número** é exatamente o que a vaga V4 do Bradesco pede quando escreve
"experiência em projetos com impacto financeiro mensurável".

---

## O que é exagero (cuidado)

### 1. "Mais de 70% esquece"
Não há fonte. É um número de efeito para chamar atenção. Não tome decisões com base nele.

### 2. "Reduzi dívida técnica em X% e entreguei ROI em Y meses"
Aqui está o principal risco para você. Em um projeto de portfólio com dados públicos **não existe empresa, então
não existe ROI real.** Se você escrever "ROI de 300% em 4 meses", a primeira pergunta da entrevista será
"como você mediu?", e não haverá resposta boa. Número inventado é pior do que número nenhum: destrói a confiança.

**O que fazer no lugar:** um **business case com hipóteses explícitas**. Exemplo:

> "Com elasticidade estimada de −0,8 e base de 1 milhão de cartões, aumentar a anuidade em 10% reduz a base em
> cerca de 8% e aumenta a receita de anuidade em cerca de 1,2%. Se a elasticidade real for −1,2, a receita cai.
> Recomendo testar o aumento em um grupo piloto antes."

Conta: receita nova ≈ 1,10 × 0,92 = 1,012 (alta de cerca de 1,2%); com −1,2: 1,10 × 0,88 = 0,968 (queda de cerca de 3,2%).
Isso é honesto, mostra raciocínio de economista e é exatamente o que um time de pricing faz no dia a dia.

### 3. "Dívida técnica"
É um conceito de engenharia de software e BI (código e painéis mal feitos que custam caro para manter).
Faz sentido para Analista de BI Sênior, que é o público do post. **Para pricing, FP&A e regulação, ninguém pergunta
sobre dívida técnica.** As vagas que você colou falam de rentabilidade, cenários, orçamento e tarifa.
Lição: o conselho foi escrito para outra vaga. Sempre confira se o público do conselho é você.

### 4. "Traga automação com agente de IA, não só Power BI"
Em 2026, "agentes de IA" é tema da moda. Nas 6 vagas, IA aparece **uma vez, como diferencial** (V3, que cita o Claude).
A automação que as vagas pedem é mais simples: "automate periodic reporting" (V1) se resolve com Power Query,
uma consulta SQL agendada ou um script Python.

Aqui entra o princípio do curso: **nem canhão para matar formiga.**

| Problema | Solução proporcional | Canhão |
|---|---|---|
| Relatório mensal que junta 5 planilhas | Power Query (atualiza com um clique) | Agente de IA que lê e-mails e monta o relatório |
| Calcular rentabilidade por cliente toda semana | Consulta SQL agendada + painel | Pipeline com LLM |
| Escrever o comentário do resultado mensal | Você escreve; IA pode ajudar no rascunho | Agente que publica sozinho |

Usar IA é bom e você já usa bastante. Mostre isso como **ferramenta de produtividade** (ex.: "usei o Claude para revisar
código e documentação"), não como o centro do projeto.

### 5. "A recrutadora só investe em profissional com entrega que resolve gargalo financeiro"
Simplificação. A triagem inicial é feita, muitas vezes, por quem confere requisitos e palavras-chave, não ROI.
O impacto financeiro pesa mais **na entrevista com o gestor**. Por isso o currículo precisa das duas coisas:
as palavras da vaga (para passar no filtro) e o resultado (para ganhar a conversa).
Ver [currículo e LinkedIn](curriculo-e-linkedin.md).

---

## Resumo em uma frase

**Fique com o esqueleto (problema → solução → impacto com número) e jogue fora a embalagem (ROI inventado,
dívida técnica e agentes de IA como enfeite).**

> ✋ **Pergunta para você:** consegue pensar em um trabalho do mestrado que você conseguiria reescrever no formato
> problema → método → impacto? Esse é um bom primeiro exercício.
