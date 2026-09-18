# Infrastructure

> Актуальность: сентябрь 2026

## Роль в системе

Где и как крутится система: сеть, хостинг, контейнеры, оркестрация, IaC, окружения, облака. Правило 2026: **PaaS → контейнеры → Kubernetes** только по необходимости, не «с первого дня».

## Что нужно знать (80/20)

- DNS, TLS, CDN, reverse proxy — часть продукта
- Модели хостинга: PaaS, VMs, containers, serverless, edge
- Иммутабельные артефакты и воспроизводимые окружения
- Секреты и конфиг отдельно от образа
- Cost и operational burden — атрибуты качества инфраструктуры

## Дочерние узлы

- [networking](./networking/)
- [hosting](./hosting/)
- [containers](./containers/)
- [orchestration](./orchestration/)
- [iac](./iac/)
- [environments](./environments/)
- [clouds](./clouds/)

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| PaaS vs k8s | Скорость команды vs контроль и портабельность |
| Single cloud vs multi-cloud | Простота vs риск vendor lock-in (часто переоценён) |

## Связанные узлы

- CI/CD: [05-cicd](../05-cicd/)
- Reliability: [06-quality/reliability](../06-quality/reliability/)
- Request path: [00-system/request-path](../00-system/request-path/)
