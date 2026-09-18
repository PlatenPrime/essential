# Containers

> Актуальность: сентябрь 2026

## Роль в системе

Упаковка приложения и зависимостей в образ: воспроизводимый артефакт для любого хоста с runtime контейнеров. База для одинаковых dev/stage/prod.

## Что нужно знать (80/20)

- Image = слои + entrypoint; tag ≠ digest (иммутабельность)
- Dockerfile best practices на уровне: multi-stage, non-root, маленький base
- Volumes, networks, env — что в образе, что снаружи
- Реестр образов; сканирование уязвимостей
- Контейнер ≠ оркестрация: один Docker Compose ≠ Kubernetes

## Дочерние узлы

- [docker](./docker/)
  - [dockerfile](./docker/dockerfile/) — слои, multi-stage, граница образа
  - [compose](./docker/compose/) — локальный стек (канон Compose)

Запланировано: image-design, registries.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Fat image vs distroless/minimal | DX отладки vs поверхность атаки и размер |
| Build in CI vs buildpacks/Nix | Контроль Dockerfile vs стандартизация платформы |

## Связанные узлы

- Orchestration: [orchestration](../orchestration/)
- Supply chain: [05-cicd/supply-chain](../../05-cicd/supply-chain/)
