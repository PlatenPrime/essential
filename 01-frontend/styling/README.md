# Styling — стратегии стилей

> Актуальность: сентябрь 2026

## Роль в системе

Как организовать CSS: глобально, модульно, utility-first, CSS-in-JS. Влияет на DX, размер бандла, runtime cost и согласованность дизайна.

## Что нужно знать (80/20)

- Каскад, specificity, cascade layers; почему «войны !important» — симптом архитектуры
- Подходы: global CSS, CSS Modules, utility (Tailwind), CSS-in-JS (runtime vs zero-runtime)
- Дизайн-токены и темизация (light/dark, бренды)
- Критический CSS и cost CSS-in-JS на runtime
- Ориентир 2026: utility-first и CSS Modules/zero-runtime чаще, чем тяжёлый runtime CSS-in-JS

## Дочерние узлы

Запланировано: tokens, utility-first, css-modules, css-in-js.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Utility-first vs semantic CSS | Скорость UI vs перенос дизайна в «имена классов» |
| Runtime CSS-in-JS vs build-time | Динамика тем vs cost на клиенте |

## Связанные узлы

- UI: [ui](../ui/)
- Perf: [performance](../performance/)
