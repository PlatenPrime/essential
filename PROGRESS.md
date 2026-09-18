# Progress — наполнение справочника

> Сейчас: Phase 5 завершена — позвоночник Ops (Docker + CI) закрыт; следующая фаза — по новому роадмапу

Правило: после каждого завершённого шага отметить `[x]` и обновить строку «Сейчас».

Новые листья позвоночника (Phase 2+) создавать сразу со схемой, если тема пространственная.

## Phase 0 — трекинг

- [x] `PROGRESS.md` + ссылка из корневого README

## Phase 1 — React spine

- [x] 1.1 `react/hooks/`
- [x] 1.2 `react/context/`
- [x] 1.3 `react/component/composition/`
- [x] 1.4 `react/component/server-client-boundary/`
- [x] 1.5 `react/component/controlled-inputs/`
- [x] 1.6 `react/patterns/`

Отложено: `concurrent/features`, `testing-components` — после meta-frameworks.

## Visuals — пилот схем (Mermaid)

- [x] конвенции: блок `## Схема` + правила Mermaid
- [x] `00-system/`, `request-path/`, `architecture-styles/`
- [x] `server-client-boundary/`, `controlled-inputs/`, `hooks/`

## Phase 2 — Meta default (Next.js)

- [x] 2.1 `meta-frameworks/nextjs/` + ссылка в родителе
- [x] 2.2 `nextjs/routing/`
- [x] 2.3 `nextjs/data-caching/`
- [x] 2.4 `nextjs/deployment-model/`
- [x] 2.5 перекрёстные ссылки + закрытие фазы

## Phase 3 — Data SoR

- [x] 3.1 `relational/postgres/` — усилить карту (схема + ссылки на листья)
- [x] 3.2 `postgres/indexing/`
- [x] 3.3 `postgres/replication/`
- [x] 3.4 `postgres/extensions/`
- [x] 3.5 `data-access/` — усилить карту (схема + ссылки на листья)
- [x] 3.6 `data-access/orm-vs-sql/`
- [x] 3.7 `data-access/migrations/`
- [x] 3.8 `data-access/transactions/`
- [x] 3.9 перекрёстные ссылки + закрытие фазы

Отложено: `serverless-postgres`, `n-plus-one` — позже по необходимости.

## Phase 4 — Auth path

- [x] 4.1 `02-backend/auth/` — усилить карту (схема + ссылки на листья)
- [x] 4.2 `auth/sessions/`
- [x] 4.3 `auth/jwt/`
- [x] 4.4 `auth/oauth-oidc/`
- [x] 4.5 `auth/rbac-abac/`
- [x] 4.6 перекрёстные ссылки с identity / security / browser
- [x] 4.7 закрытие фазы

## Phase 5 — Ops default

- [x] 5.1 `containers/docker/` — усилить карту (схема + ссылки на листья)
- [x] 5.2 `docker/dockerfile/`
- [x] 5.3 `docker/compose/`
- [x] 5.4 `cicd/platforms/` — усилить карту
- [x] 5.5 `platforms/github-actions/`
- [x] 5.6 `cicd/pipeline/` — усилить карту
- [x] 5.7 `pipeline/stages/`
- [x] 5.8 перекрёстные ссылки + закрытие фазы

Отложено: `multi-stage` как отдельный лист (покрыто в dockerfile), `gitlab-ci`, `runners`.
