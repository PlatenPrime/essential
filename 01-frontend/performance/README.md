# Performance — производительность фронта

> Актуальность: сентябрь 2026

## Роль в системе

Как быстро пользователь видит и может пользоваться UI. Архитектурные рычаги: размер JS, стратегия рендера, кэш, изображения, main-thread work.

## Что нужно знать (80/20)

- Core Web Vitals (LCP, INP, CLS) как продуктовые метрики, не «галочка Lighthouse»
- Бюджет бандла; code splitting; lazy routes/components
- Изображения: форматы, размеры, lazy, priority
- Где тормозит: сеть, JS parse/exec, layout thrashing
- Измерять в поле (RUM), не только на локальном ноуте

## Дочерние узлы

Запланировано: web-vitals, bundling, images, profiling.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Больше SSR vs меньше JS | TTFB/SEO vs сложность сервера и кэша |
| Микрофронты ради команд vs perf | Независимость деплоя vs дублирование рантаймов |

## Связанные узлы

- Рендер: [rendering](../rendering/)
- Браузер: [browser-platform](../browser-platform/)
- Observability: [06-quality/observability](../../06-quality/observability/)
