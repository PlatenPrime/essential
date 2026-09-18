# Browser platform

> Актуальность: сентябрь 2026

## Роль в системе

Среда исполнения фронта: DOM, события, сеть, storage, безопасность origin. Фреймворки стоят поверх платформы; без её модели легко принять неверные решения о кэше, auth и perf.

## Что нужно знать (80/20)

- Document / Window / Event loop (макро/микротаски) на уровне «как думает браузер»
- Same-origin policy, CORS, cookies (`HttpOnly`, `Secure`, `SameSite`)
- Storage: memory, `sessionStorage`, `localStorage`, IndexedDB, Cache API
- Сеть: fetch, HTTP/2–3, WebSocket; что блокирует main thread
- Критический путь рендера: HTML → CSS → layout → paint → composite
- Progressive enhancement и graceful degradation как архитектурные установки

## Дочерние узлы

Пока нет.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Cookie session vs token in storage | XSS-устойчивость vs удобство SPA/mobile |
| Main-thread work vs Web Workers | Простота vs отзывчивость UI |

## Связанные узлы

- Auth (канон): [02-backend/auth](../../02-backend/auth/)
- Сеть infra: [04-infrastructure/networking](../../04-infrastructure/networking/)
- Security: [06-quality/security](../../06-quality/security/)
