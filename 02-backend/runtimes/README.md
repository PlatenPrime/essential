# Runtimes — рантаймы и языки

> Актуальность: сентябрь 2026

## Роль в системе

Среда исполнения серверного кода: модель конкурентности, экосистема, деплой, найм. Выбор рантайма ограничивает фреймворки и операционную модель.

## Что нужно знать (80/20)

- **Node.js** — event loop, I/O-heavy API; TypeScript де-факто
- **Bun / Deno** — альтернативы JS-рантайма (2026: Bun зрелее в tooling; прод-HTTP часто всё ещё Node по осторожности экосистемы)
- **Python** — FastAPI/Django; силён в data/AI-сервисах
- **Go** — простота деплоя, предсказуемая конкурентность, infra-сервисы
- **JVM (Java/Kotlin)** / **.NET** — enterprise, строгая типизация, зрелый ops
- Понимать: CPU-bound vs I/O-bound workloads и что рантайм реально даёт

## Дочерние узлы

Запланировано: node, python, go, jvm, dotnet, bun.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Node vs Go для API | Скорость разработки и единый язык с фронтом vs pred. latency под нагрузкой |
| Python vs Node для AI-фич | Экосистема ML vs единый TS-стек |

## Связанные узлы

- Frameworks: [frameworks](../frameworks/)
- Infra деплой: [04-infrastructure/hosting](../../04-infrastructure/hosting/)
