# Supply chain — цепочка поставок

> Актуальность: сентябрь 2026

## Роль в системе

Безопасность зависимостей, образов и пайплайна: то, из чего собирается продукт. В 2026 сканирование в CI — baseline, не «enterprise-опция».

## Что нужно знать (80/20)

- Lockfile и воспроизводимые установки зависимостей
- SCA (Dependabot/Renovate/Snyk и аналоги); обновления как процесс
- Подпись/аттестация артефактов (идеи SLSA); pinned actions by hash
- Секреты в логах CI; OIDC к облаку вместо долгоживущих ключей
- Базовые образы и SBOM — на уровне «зачем», не сертификация

## Дочерние узлы

Запланировано: dependency-updates, image-scanning, oidc-deploy, sbom.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Auto-merge patch bots vs manual review | Скорость патчей vs риск ломающих обновлений |
| Pin by digest vs floating tags | Воспроизводимость vs удобство «latest» |

## Связанные узлы

- Security: [06-quality/security](../../06-quality/security/)
- Containers: [04-infrastructure/containers](../../04-infrastructure/containers/)
- Pipeline: [pipeline](../pipeline/)
