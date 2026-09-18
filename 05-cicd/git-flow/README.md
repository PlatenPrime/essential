# Git flow — ветвление и поставка

> Актуальность: сентябрь 2026

## Роль в системе

Как изменения попадают в main и в релиз: trunk-based, GitHub Flow, GitLab Flow, релизы. Влияет на частоту деплоя и размер PR.

## Что нужно знать (80/20)

- Trunk-based + короткоживущие ветки — ориентир высокочастотных команд
- PR как единица review и CI; размер PR влияет на качество review
- Main всегда deployable (идеал)
- Release branches / tags — когда нужны (версии, compliance)
- Merge vs squash vs rebase — командная конвенция, не религия

## Дочерние узлы

Запланировано: trunk-based, pull-requests, releases.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Trunk-based vs long-lived release branches | Скорость интеграции vs контроль релизных поездов |
| Squash merge vs merge commits | Чистая история main vs сохранение графа веток |

## Связанные узлы

- Pipeline: [pipeline](../pipeline/)
- Feature flags: [07-product-adjacent/feature-flags](../../07-product-adjacent/feature-flags/)
