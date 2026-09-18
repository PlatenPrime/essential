# Testing

> Актуальность: сентябрь 2026

## Роль в системе

Автоматическая и ручная проверка поведения. Даёт уверенность менять систему. Архитектурно: что тестировать на каком уровне.

## Что нужно знать (80/20)

- Уровни: unit, integration, e2e, contract, visual/a11y
- Пирамида / trophy: много быстрых, мало хрупких e2e
- Тест как спецификация поведения, не зеркало реализации
- Ориентир фронта 2026: Vitest + Testing Library + Playwright часто
- Тестовые данные и изоляция; флаки — долг
- Contract tests между фронтом и API / между сервисами

## Дочерние узлы

Запланировано: unit, integration, e2e, contract-tests, test-data.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Много e2e vs много integration | Уверенность «как пользователь» vs скорость и стабильность |
| Mock heavily vs test against real deps | Изоляция vs ложное чувство безопасности |

## Связанные узлы

- Pipeline: [05-cicd/pipeline](../../05-cicd/pipeline/)
- Stages (verify): [05-cicd/pipeline/stages](../../05-cicd/pipeline/stages/)
- A11y: [01-frontend/accessibility](../../01-frontend/accessibility/)
