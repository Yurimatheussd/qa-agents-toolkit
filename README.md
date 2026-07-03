# qa-agents-toolkit

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
