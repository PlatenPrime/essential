# IaC — Infrastructure as Code

> Актуальность: сентябрь 2026

## Роль в системе

Описание инфраструктуры в коде/конфиге: воспроизводимость, review, история изменений. Без IaC окружения разъезжаются.

## Что нужно знать (80/20)

- Декларативное состояние vs императивные скрипты
- Terraform/OpenTofu, cloud-native (Pulumi, CDK), платформенные шаблоны
- State: где хранится, блокировки, drift
- Модули и окружения: DRY без «божественного» monorepo-хаоса
- Секреты не коммитить; policy-as-code (идея)

## Дочерние узлы

Запланировано: terraform, pulumi, state-backends, modules.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| HCL Terraform vs general-purpose IaC | Экосистема модулей vs выразительность языка |
| One stack vs many stacks per env | Простота vs blast radius изменений |

## Связанные узлы

- Environments: [environments](../environments/)
- Clouds: [clouds](../clouds/)
- GitOps: [05-cicd/gitops](../../05-cicd/gitops/)
