# Product-adjacent — продуктовые подсистемы

> Актуальность: сентябрь 2026

## Роль в системе

Возможности, которые почти всегда есть в реальном продукте, но не равны «слою стека»: identity, платежи, уведомления, флаги, AI-фичи. Их часто покупают или подключают как сервис.

## Что нужно знать (80/20)

- Build vs buy для каждой подсистемы — отдельное архитектурное решение
- Границы: доменная логика у вас, commodity — у провайдера
- Сбои провайдера = сбои продукта; нужны деградация и идемпотентность
- Compliance (PII, платежи, AI data) влияет на выбор
- Не дублировать канон: auth API — в backend; IdP продукт — здесь

## Дочерние узлы

- [identity](./identity/)
- [payments](./payments/)
- [notifications](./notifications/)
- [feature-flags](./feature-flags/)
- [ai-features](./ai-features/)

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Build vs buy | Контроль и data ownership vs time-to-market и security burden |
| One vendor suite vs best-of-breed | Простота биллинга vs лучший fit по кускам |

## Связанные узлы

- Auth API: [02-backend/auth](../02-backend/auth/)
- Async: [02-backend/async](../02-backend/async/)
