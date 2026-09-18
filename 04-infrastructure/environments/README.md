# Environments — окружения

> Актуальность: сентябрь 2026

## Роль в системе

Разделение dev / preview / staging / prod: данные, секреты, масштаб, кто имеет доступ. Окружения — часть архитектуры поставки, не «папка на сервере».

## Что нужно знать (80/20)

- Prod-like staging vs дешёвый staging (осознанный trade-off)
- Preview environments на PR (часто с ephemeral DB)
- Конфиг и секреты per env; 12-factor идеи
- Данные: анонимизация/маскирование копий прода
- Паритет окружений снижает «у меня работает»
- Feature flags дополняют, но не заменяют env-границы

## Дочерние узлы

Запланировано: preview-envs, secrets-per-env, data-parity.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Long-lived staging vs PR previews | Стабильный QA vs изоляция веток |
| Shared DB for previews vs DB per preview | Cost vs реалистичность миграций |

## Связанные узлы

- Preview/rollout: [05-cicd/preview-rollout](../../05-cicd/preview-rollout/)
- Pipeline stages: [05-cicd/pipeline/stages](../../05-cicd/pipeline/stages/)
- Compose (local parity): [containers/docker/compose](../containers/docker/compose/)
- Feature flags: [07-product-adjacent/feature-flags](../../07-product-adjacent/feature-flags/)
- IaC: [iac](../iac/)
