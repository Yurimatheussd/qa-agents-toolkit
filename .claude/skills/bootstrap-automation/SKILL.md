---
name: bootstrap-automation
description: Monta do zero uma suíte de automação Playwright (TypeScript) para qualquer site, a partir de uma URL e parâmetros de login. Use quando o usuário pedir para criar/iniciar automação para um site novo, "montar os testes desse app", ou aplicar este padrão de automação em outro projeto.
---

Reúna do usuário (se ainda não estiver claro no pedido):
1. **URL do site** a ser automatizado.
2. **Precisa de login?** Se sim, como (usuário/senha, SSO, etc). Peça para o usuário fornecer a senha real via variável de ambiente/arquivo `.env` local, não digitada diretamente no chat.
3. **Ambiente**: produção compartilhada ou instância de teste dedicada (isso muda quão agressivo pode ser o teste).
4. **Fluxos prioritários** a cobrir primeiro, se já souber (senão, "cobertura geral" é uma resposta válida).
5. **Pasta de destino**: projeto atual ou um caminho novo/vazio.

Delegue o trabalho ao subagent `automation-bootstrapper` (via Agent tool), passando todas essas respostas.

Ao final, resuma para o usuário: a estrutura de arquivos criada (config, `support/locators.ts`, `support/pages/`, `docs/AUTOMACAO.md`, testes), o comando para rodar (`npm test` / `npm run test:headed`), e quais fluxos ficaram sem cobertura nesta primeira leva. Não repita a senha real no resumo.
