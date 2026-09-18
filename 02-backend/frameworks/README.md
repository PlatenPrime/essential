# Backend frameworks

> Актуальность: сентябрь 2026

## Роль в системе

Каркас серверного приложения: роутинг, DI, валидация, middleware, структура модулей. Задаёт конвенции команды сильнее, чем «голый» HTTP-сервер.

## Что нужно знать (80/20)

- Минимальные (Express/Fastify/Flask) vs opinionated (Nest, Django, Spring, Laravel, ASP.NET)
- Ландшафт 2026: Nest/Fastify (TS), FastAPI/Django (Python), Gin/Echo (Go), Spring Boot, ASP.NET Core, Laravel
- Что фреймворк должен дать: структура, ошибки, валидация, observability hooks, тестируемость
- «Сырой» HTTP ок для маленьких сервисов; на росте без конвенций появляется хаос

## Дочерние узлы

Запланировано: nestjs, fastapi, spring, aspnet, laravel, go-http.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Minimal vs batteries-included | Гибкость vs скорость команды и единообразие |
| MVC/fullstack vs API-only | HTML с сервера vs чистый JSON для клиентов |

## Связанные узлы

- Runtimes: [runtimes](../runtimes/)
- API styles: [api-styles](../api-styles/)
- HTML-first: [01-frontend/frameworks/html-first](../../01-frontend/frameworks/html-first/)
