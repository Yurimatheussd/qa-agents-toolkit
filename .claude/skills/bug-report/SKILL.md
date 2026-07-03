---
name: bug-report
description: Analisa falhas de teste (Playwright) ou achados de exploração deste projeto e produz um relatório de bug estruturado em reports/bugs/. Use quando o usuário pedir para investigar uma falha, triar achados, ou abrir/documentar um bug.
---

Identifique a fonte do que precisa ser triado: uma execução de teste que falhou (`test-results/`, `playwright-report/`), um achado específico de `reports/exploratory/`, ou uma descrição direta do usuário sobre algo que ele observou na app.

Delegue ao subagent `bug-hunter` (via Agent tool), passando essa fonte/contexto.

Ao final, informe ao usuário o caminho do(s) relatório(s) gerado(s) em `reports/bugs/` e a severidade atribuída.
