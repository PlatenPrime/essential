# Payments

> Актуальность: сентябрь 2026

## Роль в системе

Приём денег, подписки, счета, налоги. Почти всегда через провайдера (Stripe и аналоги); ваша зона — продуктовая модель и идемпотентность webhooks.

## Что нужно знать (80/20)

- Checkout, subscriptions, invoices; налоговые/VAT нюансы как риск
- Webhooks = источник истины о статусе платежа; проверять подпись
- Идемпотентность; reconcile расхождений
- PCI: не хранить карточные данные самому без необходимости
- Trial, proration, seat-based billing — продуктовая сложность

## Дочерние узлы

Запланировано: checkout, subscriptions, webhooks, billing-models.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Stripe-like vs regional PSP | Глобальный DX vs локальные методы оплаты |
| Billing in-house vs provider billing portal | Контроль UX vs compliance и скорость |

## Связанные узлы

- Async/webhooks: [02-backend/async](../../02-backend/async/)
- Security/PCI: [06-quality/security](../../06-quality/security/)
