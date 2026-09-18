# Analytics — аналитика и OLAP

> Актуальность: сентябрь 2026

## Роль в системе

Хранилища и пайплайны для отчётов и агрегатов: warehouse (BigQuery, Snowflake, Redshift, ClickHouse и др.), ETL/ELT. Не смешивать тяжёлую аналитику с OLTP без причины.

## Что нужно знать (80/20)

- OLTP vs OLAP нагрузки и схемы (star/snowflake — идеи)
- Batch ETL vs streaming ingestion
- Источник событий: application events, CDC из Postgres
- Product analytics (события продукта) vs BI warehouse
- Cost моделей облачных warehouse

## Дочерние узлы

Запланировано: warehouse, etl-elt, event-tracking, clickhouse.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Query OLTP replicas vs warehouse | Скорость старта vs изоляция нагрузки |
| Event stream vs nightly ETL | Свежесть метрик vs простота пайплайна |

## Связанные узлы

- Modeling: [modeling](../modeling/)
- Observability (не путать с BI): [06-quality/observability](../../06-quality/observability/)
