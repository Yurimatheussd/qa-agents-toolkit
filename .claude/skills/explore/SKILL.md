---
name: explore
description: Roda teste exploratório (não roteirizado) contra o app deste projeto, procurando comportamentos inesperados além do que a suíte automatizada já cobre. Use quando o usuário pedir para explorar a app, caçar bugs livremente, ou validar uma área específica de forma não roteirizada.
---

Se o usuário não tiver indicado uma área de foco, pergunte (ex: "votação/multiplayer", "limites de nome/sala", "espectador", "tudo de forma geral") — isso evita uma exploração genérica demais.

Delegue ao subagent `explorer` (via Agent tool), passando a área de foco (ou "exploração geral" se não houver uma).

Ao final, resuma para o usuário quantos achados foram registrados em `reports/exploratory/` e se algum parece um bug claro (nesse caso, sugira rodar a skill `/bug-report` para formalizar).
