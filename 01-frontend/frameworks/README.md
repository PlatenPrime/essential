# Frameworks — UI-фреймворки

> Актуальность: сентябрь 2026

## Роль в системе

Библиотеки/фреймворки для описания UI и реактивности. Задают модель компонентов, экосистему и кривую найма. Не путать с мета-фреймворками (роутинг, data layer, деплой).

## Что нужно знать (80/20)

- Общие идеи: компонент, props/state, декларативный UI, reconciliation / fine-grained reactivity
- Ландшафт 2026 (ориентир): React — usage-лидер; Vue — сильный DX; Angular — enterprise; Svelte/Solid — satisfaction и другая модель реактивности; HTML-first (HTMX и др.) — минимум клиентского JS
- Выбор фреймворка часто = выбор экосистемы и команды, не «бенчмарк на TodoMVC»
- TypeScript — де-факто стандарт в серьёзных UI-кодовых базах

## Дочерние узлы

- [react](./react/) — доминирующий экосистемный выбор
- [vue](./vue/)
- [angular](./angular/)
- [svelte](./svelte/)
- [solid](./solid/)
- [html-first](./html-first/) — HTMX и соседние подходы

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Virtual DOM vs fine-grained | Предсказуемость экосистемы vs меньше рантайм-оверхеда |
| Batteries-included (Angular) vs library (React) | Конвенции из коробки vs свобода сборки стека |

## Связанные узлы

- Мета-слой: [meta-frameworks](../meta-frameworks/)
- State: [state](../state/)
