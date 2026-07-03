---
name: release-notes
description: Gera release notes de um ciclo de testes deste projeto, resumindo cobertura, resultado da execução e bugs encontrados/corrigidos, salvas em reports/release-notes/. Use quando o usuário pedir release notes, um resumo do ciclo de testes, ou um relatório de qualidade de uma versão.
---

Se o usuário não tiver informado qual versão/período cobrir (ex: uma data, uma tag/versão do app, "desde a última release"), pergunte antes de prosseguir — não assuma.

Delegue ao subagent `release-notes-writer` (via Agent tool), passando a versão/período informado.

Ao final, informe ao usuário o caminho do arquivo gerado em `reports/release-notes/` e destaque a recomendação final (liberar / liberar com ressalvas / não liberar).
