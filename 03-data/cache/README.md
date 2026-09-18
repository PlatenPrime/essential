# Cache

> Актуальность: сентябрь 2026

## Роль в системе

Ускорение чтения и разгрузка primary DB: Redis и аналоги, HTTP/CDN кэш, application cache. Кэш — производный слой; источник истины остаётся в primary store.

## Что нужно знать (80/20)

- Что кэшировать: hot reads, сессии, rate limit, ephemeral locks
- TTL, eviction, stampede; инвалидация после записи
- Cache-aside vs write-through (идеи)
- Redis: структуры данных, persistence режимы, single-thread модель (концептуально)
- Опасность: кэш как «вторая БД» без политики

## Дочерние узлы

Запланировано: redis, http-caching, invalidation.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| App cache vs Redis vs CDN | Локальная простота vs shared cache vs edge |
| Short TTL vs precise invalidation | Простота vs свежесть данных |

## Связанные узлы

- Postgres: [relational/postgres](../relational/postgres/)
- Networking/CDN: [04-infrastructure/networking](../../04-infrastructure/networking/)
- Frontend data cache: [01-frontend/data-fetching](../../01-frontend/data-fetching/)
