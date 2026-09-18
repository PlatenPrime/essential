# Meta-frameworks

> Актуальность: сентябрь 2026

## Роль в системе

Слой над UI-библиотекой: файловый/конфигурируемый роутинг, data loading, SSR/SSG, API routes, адаптеры деплоя. Именно здесь часто принимают решение «как выглядит приложение целиком».

## Что нужно знать (80/20)

- Meta ≠ UI library: Next/Nuxt/SvelteKit закрывают приложение, React/Vue/Svelte — UI
- Ландшафт 2026: **Next.js** — де-факто для React и поляризующий; **Nuxt**, **SvelteKit**; **Remix / React Router** frameworks; **Astro** (content-first); **TanStack Start** и другие full-stack на Vite
- Ключевые решения: где fetch данных, где границы server/client, как деплоить (Node, serverless, edge)
- Vendor coupling: удобство хостинга vs портабельность

## Дочерние узлы

- [nextjs](./nextjs/) — де-факто meta для React: App Router, RSC, деплой

Запланировано: nuxt, sveltekit, remix, astro, tanstack-start.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Next vs Vite SPA + отдельный API | Скорость старта vs явные границы фронт/бек |
| Content-first (Astro) vs app-first (Next) | Много статики vs сильная интерактивность |
| Serverless/edge vs long-running Node | Холодный старт и лимиты vs контроль процесса |

## Связанные узлы

- Рендер: [rendering](../rendering/)
- Frameworks: [frameworks](../frameworks/)
- Хостинг: [04-infrastructure/hosting](../../04-infrastructure/hosting/)
