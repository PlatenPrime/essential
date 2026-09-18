# Pipeline

> Актуальность: сентябрь 2026

## Роль в системе

Автоматизированные шаги на изменение кода: lint, types, tests, build, security scan, deploy. Pipeline — контракт качества команды.

## Что нужно знать (80/20)

- Stages: verify → build → publish → deploy
- Fail fast; кэш зависимостей; матрицы версий осознанно
- Артефакт один и тот же для stage и prod (promote, не rebuild «чуть иначе»)
- Миграции БД: порядок относительно деплоя приложения (expand/contract)
- Секреты в CI; least privilege для deploy credentials
- Время pipeline — атрибут DX; медленный CI убивает частоту поставки

## Дочерние узлы

Запланировано: stages, caching, migrations-in-ci, artifacts.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Rebuild per env vs promote artifact | Простота vs «тот же бинарник, что тестировали» |
| All checks on every PR vs selective | Гарантии vs скорость обратной связи |

## Связанные узлы

- Platforms: [platforms](../platforms/)
- Testing: [06-quality/testing](../../06-quality/testing/)
- Supply chain: [supply-chain](../supply-chain/)
