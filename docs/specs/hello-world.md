# Spec: API Hello World

## Contexto e problema

O repositório de backend ainda não possui uma aplicação HTTP. É necessário iniciar a API com um endpoint raiz simples para confirmar que o servidor está acessível.

## Objetivo

Disponibilizar `GET /` com resposta textual `Hello World`.

## Fora de escopo

- Autenticação, autorização e multi-tenancy.
- Banco de dados, persistência e outros endpoints.
- Prefixo `/v1` para esta rota, pois o contrato solicitado é a raiz literal `/`.

## Sistemas envolvidos

- Cliente HTTP que chama a API.
- Aplicação backend NestJS.

## Comportamento esperado

- Uma requisição `GET /` retorna HTTP 200 e o texto `Hello World`.
- Nenhum outro comportamento de produto será introduzido.

## Critérios de aceitação

- CA-01: `GET /` retorna HTTP 200.
- CA-02: O corpo de `GET /` é exatamente `Hello World`.
- CA-03: A aplicação pode ser iniciada localmente por um script npm documentado no `package.json`.

## Riscos, dependências e dúvidas

- A implementação seguirá a decisão existente de NestJS e Node.js LTS.
- Não há dúvida aberta; a resposta solicitada foi interpretada como o texto `Hello World`, sem pontuação.