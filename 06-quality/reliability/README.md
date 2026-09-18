# Reliability

> Актуальность: сентябрь 2026

## Роль в системе

Способность системы выполнять работу при сбоях и нагрузке: устойчивость, деградация, восстановление. Язык: SLO, error budget, инциденты.

## Что нужно знать (80/20)

- SLO / SLI / SLA — разные понятия
- Error budget как разрешение на скорость изменений
- Паттерны: timeout, retry with jitter, circuit breaker, bulkhead, graceful degradation
- Backups и restore **проверены** учениями
- Incident response: severity, comms, postmortem без blame
- Capacity и load shedding

## Дочерние узлы

Запланировано: slo, resilience-patterns, backups, incident-response.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Multi-AZ active-active vs simpler HA | Доступность vs cost и сложность consistency |
| Auto-retry everywhere vs fail fast | Маскировка сбоев vs быстрый сигнал пользователю |

## Связанные узлы

- Observability: [observability](../observability/)
- Async retries: [02-backend/async](../../02-backend/async/)
- Rollout: [05-cicd/preview-rollout](../../05-cicd/preview-rollout/)
