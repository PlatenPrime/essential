# Hosting

> Актуальность: сентябрь 2026

## Роль в системе

Модель размещения приложения: куда деплоится процесс/функция. Определяет scaling, cold start, лимиты и связку с CI.

## Что нужно знать (80/20)

- PaaS (Vercel, Railway, Render, Fly, Heroku-like) — скорость
- VMs / bare metal — контроль и предсказуемый cost
- Containers на managed service без полного k8s
- Serverless functions / edge functions — scale-to-zero и лимиты
- Stateless app + managed data services — частый паттерн
- Vendor coupling мета-фреймворка и хостинга

## Дочерние узлы

Запланировано: paas, vms, serverless, edge.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| PaaS vs containers on VMs | Time-to-market vs контроль сети/рантайма |
| Serverless vs always-on | Cost при простое vs cold start и лимиты |

## Связанные узлы

- Containers: [containers](../containers/)
- Meta-frameworks: [01-frontend/meta-frameworks](../../01-frontend/meta-frameworks/)
- Next deployment-model: [01-frontend/meta-frameworks/nextjs/deployment-model](../../01-frontend/meta-frameworks/nextjs/deployment-model/)
- Preview deploys: [05-cicd/preview-rollout](../../05-cicd/preview-rollout/)
