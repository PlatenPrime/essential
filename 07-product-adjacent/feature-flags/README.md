# Feature flags

> Актуальность: сентябрь 2026

## Роль в системе

Отделение деплоя кода от включения функциональности: процент пользователей, сегменты, kill switch. Ускоряет поставку и снижает риск.

## Что нужно знать (80/20)

- Flag types: release, experiment, ops kill switch, permission
- Targeting: user, org, percentage, environment
- Техдолг флагов: удалять после раскатки
- Серверные vs клиентские флаги (секреты и мерцание UI)
- Связь с экспериментом (A/B), но не смешивать всё в один «божий конфиг»

## Дочерние узлы

Запланировано: flag-types, targeting, flag-debt, experimentation.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Build flags vs LaunchDarkly-like | Простота и cost vs targeting/analytics из коробки |
| Flags vs preview envs | Раскатка в prod vs изоляция незавершённого |

## Связанные узлы

- Rollout: [05-cicd/preview-rollout](../../05-cicd/preview-rollout/)
- Git flow: [05-cicd/git-flow](../../05-cicd/git-flow/)
- Environments: [04-infrastructure/environments](../../04-infrastructure/environments/)
