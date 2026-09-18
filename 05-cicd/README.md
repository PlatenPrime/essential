# CI/CD

> Актуальность: сентябрь 2026

## Роль в системе

Непрерывная проверка и доставка изменений: от push до продакшена с контролем качества и откатом. Ориентир 2026: **GitHub Actions** как массовый дефолт; GitOps — на масштабе k8s.

## Что нужно знать (80/20)

- CI (проверка) и CD (доставка) — связанные, но разные цели
- Pipeline как код; артефакты иммутабельны
- Preview → merge → prod; миграции БД в контролируемом шаге
- Rollback / forward-fix как продуктовая способность
- Supply chain: зависимости и образы тоже атакуемая поверхность

## Дочерние узлы

- [git-flow](./git-flow/)
- [pipeline](./pipeline/)
- [platforms](./platforms/)
- [preview-rollout](./preview-rollout/)
- [gitops](./gitops/)
- [supply-chain](./supply-chain/)

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Push deploy vs pull GitOps | Простота PaaS vs декларативный desired state в k8s |
| Monorepo CI vs polyrepo | Общие проверки vs независимость команд |

## Связанные узлы

- Environments: [04-infrastructure/environments](../04-infrastructure/environments/)
- Quality gates: [06-quality/testing](../06-quality/testing/)
