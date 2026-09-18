# Backend

> Актуальность: сентябрь 2026

## Роль в системе

Серверная логика: API, бизнес-правила, auth, фоновые задачи. Держит секреты, инварианты домена и границы доверия. Может быть отдельным сервисом или частью мета-фреймворка.

## Что нужно знать (80/20)

- Рантайм и язык ≠ фреймворк ≠ стиль API
- Ориентир 2026: Node/TS и Python (FastAPI) часто; Go — throughput/infra; Spring/.NET/Laravel — сильные ниши
- **Modular monolith** — частый разумный дефолт; микросервисы — отдельное решение
- Контракт API важнее выбора Express vs Fastify
- Auth, валидация входа, идемпотентность, фоновые задачи — обязательный минимум

## Дочерние узлы

- [runtimes](./runtimes/) — Node, Bun, Python, Go, JVM, …
- [frameworks](./frameworks/) — Nest, FastAPI, Spring, …
- [api-styles](./api-styles/) — REST, GraphQL, RPC
- [service-boundaries](./service-boundaries/) — нарезка и границы
- [auth](./auth/) — канон идентификации и авторизации на API
  - [sessions](./auth/sessions/), [jwt](./auth/jwt/), [oauth-oidc](./auth/oauth-oidc/), [rbac-abac](./auth/rbac-abac/)
- [async](./async/) — очереди, события, jobs

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| BFF/meta API routes vs отдельный backend | Скорость продукта vs чёткие границы и масштаб команды |
| One language full-stack vs best tool | Найм и shared types vs fit для AI/CPU/latency |

## Связанные узлы

- Стили системы: [00-system/architecture-styles](../00-system/architecture-styles/)
- Данные: [03-data](../03-data/)
- Data access: [03-data/data-access](../03-data/data-access/)
- Identity продукт: [07-product-adjacent/identity](../07-product-adjacent/identity/)
