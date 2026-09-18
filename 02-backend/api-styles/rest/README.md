# REST

> Актуальность: сентябрь 2026

## Роль в системе

Самый распространённый стиль публичных HTTP API: ресурсы, методы, статус-коды, гипермедиа опционально. На практике чаще «JSON over HTTP» с REST-дисциплиной, чем строгий Roy Fielding.

## Что нужно знать (80/20)

- Ресурсы и URI; идемпотентность методов (GET/PUT/DELETE vs POST)
- Статус-коды и единый формат ошибок
- Пагинация, фильтрация, сортировка; ETag/кэш-заголовки
- Версионирование: URL / header / evolve-by-additive
- OpenAPI как контракт и источник клиентов/валидации

## Дочерние узлы

Запланировано: versioning, pagination, openapi, caching-headers.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Strict REST vs RPC-over-HTTP | Чистые ресурсы vs «глагольные» эндпоинты под use-case |
| URL versioning vs additive evolution | Явные breaking changes vs долгая совместимость |

## Связанные узлы

- Родитель: [api-styles](../)
- GraphQL: [graphql](../graphql/)
- CDN/кэш: [04-infrastructure/networking](../../../04-infrastructure/networking/)
