# HTML-first

> Актуальность: сентябрь 2026

## Роль в системе

Подходы, где интерактивность наращивается поверх HTML/серверных шаблонов с минимумом клиентского JS (HTMX, Alpine, Unpoly и аналоги). Альтернатива rich SPA для многих CRUD/admin/контентных продуктов.

## Что нужно знать (80/20)

- Hypermedia: сервер отдаёт HTML-фрагменты, клиент подменяет части страницы
- Когда «толстый клиент» избыточен: формы, таблицы, админки, внутренние инструменты
- Trade-off: простота стека и a11y-friendly HTML vs сложные offline/rich UX
- Сочетается с классическими серверными фреймворками (Django, Rails, Laravel, Go templates)

## Дочерние узлы

Запланировано: htmx, progressive-enhancement.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| HTML-first vs SPA | Меньше JS и проще ops vs rich client и оффлайн |
| HTMX + SSR vs React meta | Команда и продукт vs экосистема и найм |

## Связанные узлы

- Рендер: [rendering](../../rendering/)
- Backend SSR: [02-backend/frameworks](../../../02-backend/frameworks/)
