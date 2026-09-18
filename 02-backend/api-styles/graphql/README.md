# GraphQL

> Актуальность: сентябрь 2026

## Роль в системе

Схема и язык запросов, где клиент выбирает форму данных. Силён при многих клиентах и сложных графах; дорог кэшем, авторизацией на поле и N+1.

## Что нужно знать (80/20)

- Schema-first: типы, queries/mutations/subscriptions
- Resolver'ы и проблема N+1 (DataLoader и аналоги)
- AuthZ на уровне типов/полей; complexity/depth limits
- Кэш сложнее, чем у REST URL (persisted queries, CDN нюансы)
- Federation / schema stitching — отдельный уровень сложности

## Дочерние узлы

Запланировано: schema-design, n-plus-one, authz, federation.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| GraphQL vs BFF REST | Гибкость одного endpoint vs простые кэшируемые ресурсы |
| Code-first vs schema-first | DX бэкенда vs контракт как источник истины |

## Связанные узлы

- API styles: [api-styles](../)
- Data access: [03-data/data-access](../../../03-data/data-access/)
