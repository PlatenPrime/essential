# Orchestration

> Актуальность: сентябрь 2026

## Роль в системе

Запуск многих контейнеров: расписание, health, scaling, networking, секреты. Kubernetes — стандарт индустрии на масштабе; на старте часто избыточен.

## Что нужно знать (80/20)

- Задачи оркестратора: placement, restart, service discovery, rolling update
- Kubernetes: Pod/Deployment/Service/Ingress — карта понятий, не сертификация
- Managed k8s (EKS/GKE/AKS) vs «свой кластер»
- Альтернативы проще: Docker Compose, Nomad, платформенные контейнерные сервисы
- GitOps часто идёт в паре с k8s (см. CI/CD)

## Дочерние узлы

Запланировано: kubernetes-basics, managed-k8s, when-not-k8s.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| K8s vs PaaS/containers service | Портабельность и контроль vs операционная нагрузка |
| Ingress controller vs cloud LB | Гибкость маршрутизации vs нативная интеграция облака |

## Связанные узлы

- Containers: [containers](../containers/)
- GitOps: [05-cicd/gitops](../../05-cicd/gitops/)
- Reliability: [06-quality/reliability](../../06-quality/reliability/)
