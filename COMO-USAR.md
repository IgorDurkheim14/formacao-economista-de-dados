# Como usar este repositório

> 📍 Você está em: [início](README.md) › **Como usar**

Este guia responde: **onde ficam os arquivos, como abrir, como salvar o progresso e como continuar em outro computador.**

## 1. Entendendo as três "cópias"

Pense no repositório como um caderno que existe em dois lugares:

| Onde | O que é | Analogia |
|---|---|---|
| **GitHub** (`github.com/IgorDurkheim14/formacao-economista-de-dados`) | A cópia oficial, na nuvem | O caderno guardado no cofre |
| **Seu computador** (a pasta clonada) | A cópia em que você trabalha | O caderno aberto na mesa |
| **Histórico (commits)** | Cada "foto" salva do caderno | As páginas datadas |

Você trabalha no computador e, ao final, **envia** (push) para o GitHub. Em outro computador, você **baixa** (clone na primeira vez, pull nas próximas).

## 2. Três maneiras de usar (escolha a sua)

### Maneira A: só pelo navegador (mais simples, zero instalação)
- Abra `github.com/IgorDurkheim14/formacao-economista-de-dados`, navegue pelas pastas, leia os READMEs.
- Para editar: abra o arquivo → ícone de lápis ✏️ → edite → **Commit changes**.
- Para uma tela de editor completa: aperte a tecla **`.`** (ponto) dentro do repositório. Abre o VS Code no navegador.
- **Bom para:** anotações e diário. **Ruim para:** rodar código Python.

### Maneira B: GitHub Desktop (recomendada para começar)
1. Instale o [GitHub Desktop](https://desktop.github.com/) e entre com sua conta.
2. **File → Clone repository** → escolha `formacao-economista-de-dados` → escolha a pasta (sugestão: `Documentos/GitHub/`).
3. Trabalhe normalmente nos arquivos dessa pasta (VS Code, Excel, Jupyter...).
4. Ao terminar: no GitHub Desktop, escreva um resumo (ex.: `SQL: exercícios de JOIN`) → **Commit to main** → **Push origin**.
5. No outro computador: clone uma vez; nas próximas vezes clique em **Fetch origin / Pull** antes de começar.

### Maneira C: terminal (o que o mercado usa, aprenda na Fase 5)
```bash
# primeira vez em um computador
git clone https://github.com/IgorDurkheim14/formacao-economista-de-dados.git
cd formacao-economista-de-dados

# toda vez que for começar a estudar
git pull

# toda vez que terminar
git add .
git commit -m "SQL: exercícios de JOIN"
git push
```

## 3. A rotina de cada sessão de estudo

```
ANTES  →  Pull (pegar a versão mais recente)
DURANTE → Estudar, salvar anotações/exercícios na pasta do módulo
DEPOIS →  Registrar no diário (progresso/diario/) → Commit → Push
```

> ⚠️ **Regra de ouro:** sempre faça **Pull antes** e **Push depois**. Assim os dois computadores nunca ficam com versões diferentes.

## 4. Onde salvar cada tipo de arquivo

| Tipo de arquivo | Onde vai | Exemplo |
|---|---|---|
| Resumo / anotação | `<fase>/<módulo>/anotacoes/` | `01-fundamentos/01-sql/anotacoes/joins.md` |
| Exercício | `<fase>/<módulo>/exercicios/` | `.../exercicios/ex01-select-basico.sql` |
| Mini-projeto | `<fase>/<módulo>/projeto/` | `.../projeto/README.md` + arquivos |
| Registro de estudo | `progresso/diario/` | `progresso/diario/2026-11-20.md` |
| Dados pequenos (< 10 MB) | `dados/brutos/` ou `dados/tratados/` | `dados/brutos/ipca.csv` |
| Dados grandes | **Fora do GitHub** (Drive) + link em `dados/README.md` | |
| Projeto pronto para mostrar | `portfolio/` (resumo + link) | |

### Padrão de nomes
- Tudo minúsculo, sem acento, palavras separadas por hífen: `analise-vendas-2025.ipynb`.
- Exercícios numerados: `ex01-...`, `ex02-...`.
- Diário com data no formato ano-mês-dia: `2026-11-20.md` (assim fica em ordem automaticamente).

## 5. Formato `.md` (Markdown): por que quase tudo é assim?
Arquivos `.md` são texto simples que o GitHub mostra formatado (títulos, listas, tabelas).
- `# Título`, `## Subtítulo`
- `- item de lista`, `- [ ] tarefa` / `- [x] tarefa feita`
- `**negrito**`, `` `código` ``

Vantagem: abre em qualquer computador, em qualquer programa, e o Git mostra exatamente o que mudou.

## 6. Problemas comuns
| Problema | O que fazer |
|---|---|
| "Push rejected" | Faça **Pull** primeiro, depois Push de novo. |
| Arquivo muito grande | Tire o arquivo da pasta, guarde no Drive e coloque o link em `dados/README.md`. |
| Apaguei algo sem querer | Ainda não fez commit? Desfaça no GitHub Desktop (botão direito → Discard). Já fez? O histórico guarda tudo, me peça ajuda para recuperar. |
