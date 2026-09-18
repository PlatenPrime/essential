# Notifications

> Актуальность: сентябрь 2026

## Роль в системе

Доставка сообщений пользователю: email, push, SMS, in-app. Обычно очередь + провайдер; шаблоны и предпочтения — продуктовая логика.

## Что нужно знать (80/20)

- Каналы и их failure modes (bounce, unsubscribe, quiet hours)
- Transactional vs marketing (и consent)
- Шаблоны, локализация, idempotent send
- Провайдеры (SendGrid, SES, Postmark, OneSignal, …) vs SMTP self-host
- Наблюдаемость доставки; не блокировать HTTP-запрос на send

## Дочерние узлы

Запланировано: email, push, sms, preferences.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Direct provider API vs notification service | Простота vs единый слой предпочтений/каналов |
| Sync send vs queue | Простота кода vs latency и retries |

## Связанные узлы

- Async: [02-backend/async](../../02-backend/async/)
- Reliability: [06-quality/reliability](../../06-quality/reliability/)
