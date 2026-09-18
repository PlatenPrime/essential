# Quality

> Актуальность: сентябрь 2026

## Роль в системе

Как система остаётся правильной, наблюдаемой, безопасной и устойчивой. Качество — сквозной слой: тесты, telemetry, security, reliability. Без него архитектура «на бумаге».

## Что нужно знать (80/20)

- Пирамида тестов и стоимость обратной связи
- Observability: logs, metrics, traces — чтобы чинить то, что измерили
- Security — процесс и поверхность атаки, не разовый audit
- Reliability: SLO/error budget как язык договорённостей
- Качество встраивается в CI и в дизайн, не «отдел в конце»

## Дочерние узлы

- [testing](./testing/)
- [observability](./observability/)
- [security](./security/)
- [reliability](./reliability/)

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Coverage % vs risk-based tests | Метрика для галочки vs тесты на дорогие сбои |
| Shift-left security vs perimeter only | Дешевле чинить рано vs «файрвол спасёт» |

## Связанные узлы

- CI gates: [05-cicd/pipeline](../05-cicd/pipeline/)
- Quality attributes: [00-system/quality-attributes](../00-system/quality-attributes/)
