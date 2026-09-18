# Relational — реляционные СУБД

> Актуальность: сентябрь 2026

## Роль в системе

Таблицы, SQL, ACID, связи. Дефолт для большинства бизнес-приложений. В 2026 PostgreSQL часто закрывает и JSON, FTS, vectors (pgvector) — «Postgres for many things».

## Что нужно знать (80/20)

- Ключи, индексы, JOIN, транзакции и уровни изоляции (на уровне решений)
- Миграции схемы; downtime vs online migrations
- Connection pooling; read replicas и их consistency
- JSONB и расширения — сила Postgres, не повод игнорировать реляцию
- MySQL/MariaDB и облачные ветвления (PlanetScale и аналоги) — отдельные ветки экосистемы

## Дочерние узлы

- [postgres](./postgres/) — де-факто system of record

Запланировано: mysql, migrations, indexing.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Managed Postgres vs self-host | Скорость и бэкапы vs контроль и cost |
| SQL-first vs «DB as dumb store» | Инварианты в БД vs вся логика в приложении |

## Связанные узлы

- Modeling: [modeling](../modeling/)
- Cache: [cache](../cache/)
- Data access: [data-access](../data-access/)
