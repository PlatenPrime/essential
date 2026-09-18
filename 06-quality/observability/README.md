# Observability

> Актуальность: сентябрь 2026

## Роль в системе

Способность понять состояние системы по данным снаружи: логи, метрики, трейсы, профили. Без этого инциденты гадаются.

## Что нужно знать (80/20)

- Three pillars (+ continuous profiling как дополнение)
- Structured logs; correlation / trace id сквозь сервисы и async
- RED/USE метрики; SLI из метрик пользователя
- Distributed tracing для path запроса
- Cardinality и cost телеметрии
- Alerting на симптомы для пользователя, не на «диск 80%» в вакууме

## Дочерние узлы

Запланировано: logging, metrics, tracing, alerting.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Vendor APM vs open stack (OTel) | Скорость старта vs портабельность и cost |
| Log everything vs sample traces | Полнота vs счёт и шум |

## Связанные узлы

- Request path: [00-system/request-path](../../00-system/request-path/)
- Reliability: [reliability](../reliability/)
- Frontend perf RUM: [01-frontend/performance](../../01-frontend/performance/)
