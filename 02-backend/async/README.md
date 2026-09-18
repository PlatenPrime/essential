# Async — фоновая работа и события

> Актуальность: сентябрь 2026

## Роль в системе

Всё, что не обязано уложиться в один HTTP-ответ: очереди, workers, cron, webhooks, domain events. Снижает связность и latency запроса ценой eventual consistency и операционной сложности.

## Что нужно знать (80/20)

- Job queue vs pub/sub vs event log (Kafka и аналоги)
- At-least-once доставка → идемпотентные обработчики
- Outbox / inbox для согласованности с БД
- Dead letter, retry backoff, poison messages
- Наблюдаемость: correlation id через async границы
- Когда async обязателен: email, биллинг, тяжёлые отчёты, интеграции

## Дочерние узлы

Запланировано: queues, events, outbox, scheduling.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Sync call vs queue | Простота отладки vs устойчивость к пикам и сбоям |
| Broker (Kafka) vs lightweight queue (Redis/SQS) | Throughput/replay vs операционная простота |

## Связанные узлы

- Boundaries: [service-boundaries](../service-boundaries/)
- Reliability: [06-quality/reliability](../../06-quality/reliability/)
- Notifications: [07-product-adjacent/notifications](../../07-product-adjacent/notifications/)
