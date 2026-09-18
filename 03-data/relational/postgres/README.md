# PostgreSQL

> Актуальность: сентябрь 2026

## Роль в системе

Самый частый выбор OLTP system of record в веб/SaaS 2026. Зрелая SQL-СУБД + JSONB, FTS, расширения (PostGIS, pgvector). Уметь «думать Postgres» важнее, чем знать все флаги.

## Что нужно знать (80/20)

- Роль: источник истины, транзакции, ограничения целостности
- Индексы (B-tree и когда нужны другие), EXPLAIN на уровне «уметь читать»
- MVCC и следствия для long transactions / bloat (концептуально)
- Пул соединений (PgBouncer и аналоги); лимиты serverless Postgres
- Бэкапы, PITR, реплики — часть архитектуры, не «потом ops»
- Когда выносить нагрузку: кэш, search, OLAP, отдельный vector store

## Дочерние узлы

Запланировано: indexing, replication, extensions, serverless-postgres.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Vanilla Postgres vs Supabase/Neon-style | Контроль vs auth/storage/branching из коробки |
| pgvector in Postgres vs dedicated vector DB | Операционная простота vs спец. масштаб embeddings |

## Связанные узлы

- Relational: [relational](../)
- Vectors: [vectors](../../vectors/)
- Environments/preview DB: [04-infrastructure/environments](../../../04-infrastructure/environments/)
