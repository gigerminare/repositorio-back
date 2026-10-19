# Plano: API Hello World

## Arquivos

- `package.json`: dependências e scripts de desenvolvimento, teste e build.
- `tsconfig.json` e `nest-cli.json`: configuração mínima de TypeScript e NestJS.
- `src/main.ts`: inicialização HTTP local.
- `src/app.module.ts`, `src/app.controller.ts` e `src/app.service.ts`: módulo e rota raiz.
- `test/app.e2e-spec.ts` e `test/jest-e2e.json`: teste HTTP do contrato.
- `docs/specs/hello-world.md`: comportamento e critérios de aceitação.
- `tasks/hello-world.md`: execução e rastreabilidade.

## Abordagem

1. Inicializar um projeto NestJS enxuto, compatível com a stack já decidida.
2. Implementar somente `GET /` com a resposta `Hello World`.
3. Validar status e corpo da resposta com Jest e supertest.

## Verificação

- Executar o teste E2E do endpoint.
- Executar o build TypeScript/NestJS.
- Confirmar que o script `start:dev` inicia o servidor local.
- Executar `git diff --check` e revisar `git status --short`.

## Impacto e rastreabilidade

- CA-01 e CA-02: controller/service e teste E2E.
- CA-03: scripts npm e inicialização local.
- Sem impacto em dados, autenticação ou contratos existentes.