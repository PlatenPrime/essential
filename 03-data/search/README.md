# Search

> Актуальность: сентябрь 2026

## Роль в системе

Полнотекстовый и фасетный поиск: Elasticsearch/OpenSearch, Typesense, Meilisearch, или FTS в Postgres. Отдельный индекс почти всегда eventual относительно OLTP.

## Что нужно знать (80/20)

- Search ≠ SQL `LIKE`: токены, релевантность, ranking
- Синхронизация индекса с primary (двойная запись, CDC, outbox)
- Когда хватает Postgres FTS / `pg_trgm`, а когда нужен движок
- Анализаторы языка, опечатки, фильтры — продуктовые решения
- Ops стоимость кластера поиска

## Дочерние узлы

Запланировано: full-text-postgres, opensearch, sync-strategies.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Postgres FTS vs dedicated search | Простота ops vs релевантность и масштаб |
| Sync index sync vs async | Свежесть vs нагрузка на запись |

## Связанные узлы

- Async sync: [02-backend/async](../../02-backend/async/)
- Postgres: [relational/postgres](../relational/postgres/)
