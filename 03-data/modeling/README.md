# Modeling — моделирование данных

> Актуальность: сентябрь 2026

## Роль в системе

Как представить домен в хранилище: сущности, связи, инварианты, эволюция схемы. Ошибки модели дороже выбора ORM.

## Что нужно знать (80/20)

- Нормализация vs денормализация под read-модели
- Aggregate / bounded context (хотя бы на уровне идей DDD)
- Strong vs eventual consistency; где нужны транзакции
- Миграции как продукт: expand/contract, backward compatibility — см. [data-access/migrations](../data-access/migrations/)
- Идентификаторы: surrogate vs natural; UUID/ULID и индексы
- Мягкое удаление, аудит, мультитенантность — заранее

## Дочерние узлы

Запланировано: normalization, consistency, multi-tenancy.

Стратегия миграций — канонически в [data-access/migrations](../data-access/migrations/).

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Normalized OLTP vs read-model | Целостность записи vs скорость чтения |
| Shared schema vs schema per tenant | Простота ops vs изоляция и кастомизация |

## Связанные узлы

- Relational: [relational](../relational/)
- Data access: [data-access](../data-access/)
- Migrations: [data-access/migrations](../data-access/migrations/)
- Transactions: [data-access/transactions](../data-access/transactions/)
- Boundaries: [02-backend/service-boundaries](../../02-backend/service-boundaries/)
