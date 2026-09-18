# React

> Актуальность: сентябрь 2026

## Роль в системе

Самый распространённый UI-фреймворк по usage. Задаёт экосистему (мета-фреймворки, data libraries, hiring). Архитектурно важно понимать модель компонентов, границы server/client и стоимость абстракций.

## Что нужно знать (80/20)

- Компонент как единица UI; props вниз, события/колбэки вверх
- Рендер = функция состояния; побочные эффекты отделены (effects)
- Ключи списков, контролируемые/неконтролируемые инпуты
- Граница **client** vs **server** components в современных мета-стеках
- Экосистема: роутинг и data часто живут в meta-framework / TanStack Query, а не «в чистом React»
- React ≠ Next.js: библиотека UI vs полный фреймворк приложения

## Дочерние узлы

- [component](./component/) — эталонный лист: что знать о компоненте
- [hooks](./hooks/) — переиспользование логики: state, effects, кастомные хуки
- [context](./context/) — проброс зависимостей без prop drilling
- [patterns](./patterns/) — compound, controlled API, headless

Запланировано (без папок пока): concurrent/features.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| SPA на Vite vs Next/Remix | Контроль сборки vs встроенные SSR/маршруты/деплой |
| Local state vs server cache | Где правда о данных: UI или бэкенд |

## Связанные узлы

- Рендер: [rendering](../../rendering/)
- Мета: [meta-frameworks](../../meta-frameworks/)
- Data fetching: [data-fetching](../../data-fetching/)
