---
name: write-tests
description: Escreve ou atualiza specs Playwright (TypeScript puro, sem BDD/Gherkin) para a suíte deste projeto. Use quando o usuário pedir para adicionar cobertura de teste, automatizar um fluxo, ou ajustar um teste existente.
---

Reúna do usuário (se ainda não estiver claro no pedido) qual funcionalidade/fluxo deve ser coberto, e se há um caso específico em mente ou se é pra cobrir a área de forma geral (nesse caso, consulte a seção "Sugestões de cenários" de `docs/AUTOMACAO.md`).

Delegue o trabalho ao subagent `test-writer` (via Agent tool) passando:
- a descrição do fluxo/caso a cobrir
- se é um arquivo novo em `tests/` ou alteração de um existente
- qualquer detalhe que o usuário já tenha dado sobre o comportamento esperado

Depois que o subagent retornar, resuma para o usuário: o que foi criado/alterado, e se `npx playwright test` passou.
