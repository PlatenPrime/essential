# Data

> Актуальность: сентябрь 2026

## Роль в системе

Хранение и доступ к данным: модель, транзакции, специализированные хранилища. Ориентир 2026: **PostgreSQL** как system of record; рядом Redis, search, analytics, vectors по нагрузке — не «вместо».

## Что нужно знать (80/20)

- Сначала **access patterns** и consistency, потом бренд БД
- OLTP vs OLAP; operational DB ≠ warehouse
- Транзакции, изоляции, миграции схемы — часть продукта
- Кэш — не источник истины; инвалидация сложнее записи
- Полиглот persistence оправдан разными нагрузками, не модой

## Дочерние узлы

- [modeling](./modeling/) — моделирование и consistency
- [relational](./relational/) — SQL / Postgres
- [document](./document/) — документные СУБД
- [cache](./cache/) — Redis и кэш-слои
- [search](./search/) — полнотекст и search engines
- [analytics](./analytics/) — OLAP / warehouse
- [vectors](./vectors/) — embeddings / semantic search
- [data-access](./data-access/) — ORM, SQL, миграции

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| One Postgres vs many specialized stores | Операционная простота vs fit нагрузки |
| Schema-on-write vs flexible documents | Инварианты в БД vs скорость эволюции формы |

## Связанные узлы

- Backend: [02-backend](../02-backend/)
- Quality attributes: [00-system/quality-attributes](../00-system/quality-attributes/)
