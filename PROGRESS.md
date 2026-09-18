# Progress — наполнение справочника

> Сейчас: Phase 2 завершена — следующий фокус Phase 3 (Data SoR), после короткого роадмапа

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

## Phase 3 — Data SoR (роадмап перед стартом)

- [ ] детальный чеклист перед стартом
- [ ] postgres: indexing, replication, extensions
- [ ] data-access: orm-vs-sql, migrations, transactions

## Phase 4 — Auth path (роадмап перед стартом)

- [ ] детальный чеклист перед стартом
- [ ] auth: sessions, jwt, oauth-oidc, rbac-abac
- [ ] перекрёстные ссылки с identity

## Phase 5 — Ops default (роадмап перед стартом)

- [ ] детальный чеклист перед стартом
- [ ] docker: dockerfile, compose
- [ ] cicd: github-actions (+ stages при необходимости)
