# GitOps

> Актуальность: сентябрь 2026

## Роль в системе

Желаемое состояние инфраструктуры/деплоя хранится в git; агент (Argo CD, Flux) приводит кластер к нему. Типично для Kubernetes; не обязателен на PaaS.

## Что нужно знать (80/20)

- Pull-based reconcile vs push deploy из CI
- Git как audit log изменений среды
- Разделение app repo и env/config repo (часто)
- Секреты: sealed secrets, external secrets — отдельная задача
- Drift detection: ручные kubectl apply ломают модель

## Дочерние узлы

Запланировано: argo-cd, flux, app-of-apps, secrets.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| GitOps vs CI push deploy | Декларативность и drift control vs простота пайплайна |
| Mono-repo envs vs repo-per-env | Обзорность vs права доступа и blast radius |

## Связанные узлы

- Orchestration: [04-infrastructure/orchestration](../../04-infrastructure/orchestration/)
- IaC: [04-infrastructure/iac](../../04-infrastructure/iac/)
- Pipeline: [pipeline](../pipeline/)
