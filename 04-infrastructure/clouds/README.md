# Clouds

> Актуальность: сентябрь 2026

## Роль в системе

Провайдеры инфраструктуры и managed-сервисов (AWS, GCP, Azure, и «альтернативы»: Hetzner, Cloudflare, …). Выбор = экосистема сервисов, IAM, регионы, cost model.

## Что нужно знать (80/20)

- IaaS / PaaS / managed data — разные уровни ответственности
- IAM и границы аккаунтов/проектов — security-критично
- Регионы, зоны доступности, latency и data residency
- Account/org structure (landing zone) на росте
- FinOps: видеть cost драйверы (egress, DB, k8s)
- Multi-cloud редко нужен «для надёжности»; чаще — разные инструменты (CDN + compute)

## Дочерние узлы

Запланировано: aws, gcp, azure, cloudflare, cost-model.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Hyperscaler vs simpler VPS+managed DB | Ширина сервисов vs предсказуемый cost и простота |
| One account vs multi-account | Простота старта vs изоляция blast radius |

## Связанные узлы

- Hosting: [hosting](../hosting/)
- IaC: [iac](../iac/)
- Security: [06-quality/security](../../06-quality/security/)
