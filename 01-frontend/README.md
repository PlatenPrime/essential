# Frontend

> Актуальность: сентябрь 2026

## Роль в системе

Слой взаимодействия с пользователем: UI, рендер, клиентское состояние, загрузка данных. Определяет UX, SEO, размер бандла и то, где выполняется код (браузер / сервер / edge).

## Что нужно знать (80/20)

- Браузер — платформа со своим runtime (DOM, сеть, storage, security model)
- Модели рендера: CSR, SSR, SSG, streaming, RSC — это **где** и **когда** строится UI
- Фреймворк UI ≠ мета-фреймворк (маршруты, data, деплой)
- State бывает: локальный UI, серверный кэш, URL, глобальный клиентский
- Perf и a11y — не «потом», а часть архитектуры фронта
- Ориентир 2026: React доминирует по usage; Vue/Svelte сильны по satisfaction; Next.js — де-факто и поляризующий

## Дочерние узлы

- [browser-platform](./browser-platform/) — платформа браузера
- [rendering](./rendering/) — модели рендера
- [frameworks](./frameworks/) — UI-фреймворки
- [meta-frameworks](./meta-frameworks/) — Next, Nuxt, SvelteKit, Astro, …
- [ui](./ui/) — компоненты, дизайн-системы
- [state](./state/) — управление состоянием
- [data-fetching](./data-fetching/) — загрузка и кэш серверных данных
- [styling](./styling/) — CSS-стратегии
- [performance](./performance/) — Core Web Vitals, бандл
- [accessibility](./accessibility/) — a11y как требование

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| SPA vs meta-framework | Контроль клиента vs батареи SSR/маршрутов/деплоя из коробки |
| React vs Vue/Svelte/Solid | Экосистема и найм vs модель реактивности и DX |
| HTML-first vs heavy JS | Минимальный JS (HTMX и др.) vs rich client |

## Связанные узлы

- Путь запроса: [00-system/request-path](../00-system/request-path/)
- API контракты: [02-backend/api-styles](../02-backend/api-styles/)
- Качество фронта: [06-quality/testing](../06-quality/testing/)
