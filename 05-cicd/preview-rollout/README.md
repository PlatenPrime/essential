# Preview & rollout

> Актуальность: сентябрь 2026

## Роль в системе

Как показывать изменения до прода и как выкатывать на прод: preview URL, canary, blue-green, progressive delivery. Снижает риск деплоя.

## Что нужно знать (80/20)

- Preview deploy на PR — быстрый feedback (часто у PaaS)
- Rollout стратегии: recreate, rolling, blue-green, canary
- Feature flags vs deploy: разделение «доставить код» и «включить фичу»
- Миграции и совместимость old/new app во время rollout
- Rollback: умение откатиться быстрее, чем «긴급чный hotfix»

## Дочерние узлы

Запланировано: preview-deploys, canary, blue-green, rollback.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Preview every PR vs shared staging | Изоляция vs cost и данные |
| Canary vs feature flag | Инфра-процент трафика vs продуктовый таргетинг |

## Связанные узлы

- Environments: [04-infrastructure/environments](../../04-infrastructure/environments/)
- Feature flags: [07-product-adjacent/feature-flags](../../07-product-adjacent/feature-flags/)
- Reliability: [06-quality/reliability](../../06-quality/reliability/)
