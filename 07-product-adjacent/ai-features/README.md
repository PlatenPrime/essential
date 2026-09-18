# AI features

> Актуальность: сентябрь 2026

## Роль в системе

LLM и ML как **компонент продукта**: генерация, поиск, классификация, агенты. Архитектурно — ещё один ненадёжный внешний сервис с cost и политикой данных.

## Что нужно знать (80/20)

- Модель как dependency: latency, cost, rate limits, versioning
- RAG: документы → chunks → vectors → prompt; оценка качества
- Prompt/versioning; evals важнее «поигрались в чате»
- Границы доверия: не выполнять сырой tool-output без проверок
- PII и retention у провайдера модели; on-prem/VPC варианты
- Fallback и деградация, когда модель недоступна

## Дочерние узлы

Запланировано: rag, evals, agents-tools, model-providers.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| API foundation model vs self-host | Скорость и качество vs data control и cost at scale |
| RAG vs fine-tune | Актуальность знаний vs специализация поведения |

## Связанные узлы

- Vectors: [03-data/vectors](../../03-data/vectors/)
- Async jobs: [02-backend/async](../../02-backend/async/)
- Security/data: [06-quality/security](../../06-quality/security/)
