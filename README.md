# qa-agents-toolkit

Conjunto de subagentes Claude Code para automação de QA — bootstrap de suítes Playwright, escrita de testes, exploração livre, triagem de bugs e geração de release notes.

## Agentes

- **automation-bootstrapper** — monta do zero uma suíte de automação Playwright (TypeScript) para qualquer site.
- **test-writer** — escreve ou atualiza specs de teste Playwright em uma suíte já existente.
- **explorer** — roda testes exploratórios livres contra uma aplicação web, caçando casos extremos que os testes roteirizados não cobrem.
- **bug-hunter** — analisa falhas de teste e achados de exploração, produzindo relatórios de bug estruturados.
- **release-notes-writer** — gera release notes resumindo a cobertura de testes e os bugs encontrados/corrigidos em um ciclo.

## Skills

Cada agente tem uma skill (slash-command) correspondente em `.claude/skills/`:

- `bootstrap-automation`
- `write-tests`
- `explore`
- `bug-report`
- `release-notes`

## Uso

Copie `.claude/agents/` e `.claude/skills/` para qualquer projeto para habilitar esses agentes e skills nele.

---

# qa-agents-toolkit (English)

Claude Code subagents that bootstrap, test, explore, and report on QA automation suites (Playwright/TS).

## Agents

- **automation-bootstrapper** — scaffolds a brand-new Playwright (TypeScript) automation suite from scratch for any target website.
- **test-writer** — writes or updates Playwright test specs for an already-scaffolded suite.
- **explorer** — runs free-form exploratory testing against a web app, hunting for edge cases not covered by scripted tests.
- **bug-hunter** — analyzes test failures and exploratory findings, producing structured bug reports.
- **release-notes-writer** — generates release notes summarizing test coverage and bugs found/fixed for a test cycle.

## Skills

Each agent has a matching slash-command skill under `.claude/skills/`:

- `bootstrap-automation`
- `write-tests`
- `explore`
- `bug-report`
- `release-notes`

## Usage

Copy `.claude/agents/` and `.claude/skills/` into any project to enable these agents and skills there.
