# Data fetching — загрузка данных

> Актуальность: сентябрь 2026

## Роль в системе

Как клиент (или серверный рендер) получает данные API: кэш, ревалидация, ошибки, гонки запросов. Связывает фронт с контрактами бека.

## Что нужно знать (80/20)

- Fetch на mount vs loader/SSR prefetch vs RSC/server fetch
- Кэш, stale-while-revalidate, инвалидация после мутаций
- Обработка loading / error / empty; отмена и dedupe запросов
- Граница: что можно кэшировать на CDN/edge, что только приватно
- Контракт API (типы, ошибки, пагинация) важнее выбора HTTP-клиента

## Дочерние узлы

Запланировано: caching, mutations, ssr-prefetch, realtime.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Client fetch vs server fetch | Интерактивность и кэш браузера vs секреты и TTFB |
| REST resource cache vs GraphQL client cache | Простота URL vs гибкость запросов и нормализация |

## Связанные узлы

- API: [02-backend/api-styles](../../02-backend/api-styles/)
- State: [state](../state/)
- Рендер: [rendering](../rendering/)
