# Diagnóstico: problema → ferramenta

> 📍 Você está em: [início](../../README.md) › [Fase 0 · Orientação e diagnóstico](../README.md) › **Diagnóstico: problema → ferramenta**

**Status:** ⬜ não iniciado  <!-- troque por 🟨 em andamento ou ✅ concluído -->

## 1. O que é?
O método de escolher a solução mais simples que resolve: planilha, SQL, painel, script ou modelo.

## 2. Por que estou estudando isso?
É o que separa um operador de ferramentas de alguém que resolve problemas.

## 3. Quando usar (e quando NÃO usar)?
Antes de começar qualquer análise ou projeto.

## 4. Com o que se conecta?
É o critério usado em todo módulo, na seção "Quando usar e quando NÃO usar".

---

## O que tem nesta pasta

| Pasta | Para que serve |
|---|---|
| `anotacoes/` | Resumos com suas palavras. Um arquivo por tema (ex.: `joins.md`). |
| `exercicios/` | Exercícios resolvidos, com o enunciado no topo do arquivo. |
| `projeto/` | O mini-projeto do módulo, com README próprio (use o modelo em `templates/`). |

## Checklist do módulo
- [ ] Conceitos principais estudados (resumo em `anotacoes/`)
- [ ] Pelo menos 10 exercícios resolvidos em `exercicios/`
- [ ] Mini-projeto feito em `projeto/`
- [ ] Registro no diário de bordo (`progresso/diario/`)

## Materiais usados
_Anote aqui cursos, vídeos, livros e links que você usou neste módulo._
-


## Exemplo do método (para começar)

**Situação:** o gestor pergunta "quanto vendemos por região no último trimestre?"

| Pergunta de diagnóstico | Resposta | Ferramenta indicada |
|---|---|---|
| É uma pergunta única ou vai se repetir? | Única | Não precisa automatizar |
| Onde estão os dados? | Num banco de dados | SQL |
| Quantas linhas? | 50 mil | SQL resume; Excel aguenta o resultado |
| Quem vai usar? | Gestor, uma vez | Uma tabela no Excel ou um print basta |

**Solução simples:** uma consulta SQL com `GROUP BY regiao` e o resultado colado no Excel.

**Agora se a pergunta for toda semana:** a mesma consulta vira fonte de um painel Power BI que atualiza sozinho. Mesma pergunta, frequência diferente, ferramenta diferente.

**E se a pergunta virar "a campanha de outubro aumentou as vendas?":** aí não é mais descrição, é causalidade. Entra a inferência causal (Fase 4).

## A escada de soluções (da mais simples à mais complexa)
1. Conversar / olhar o dado na fonte
2. Planilha (Excel)
3. Consulta SQL
4. Painel (Power BI)
5. Script Python (automação, limpeza pesada, econometria)
6. Modelo estatístico / ML
7. App publicado (deploy)

Suba um degrau só quando o anterior não resolve bem.
