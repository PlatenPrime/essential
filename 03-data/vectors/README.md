# Vectors — векторный поиск

> Актуальность: сентябрь 2026

## Роль в системе

Хранение embeddings и semantic search для AI-фич. В 2026 часто начинают с **pgvector** в Postgres; отдельные vector DB — при масштабе или спец. требованиях.

## Что нужно знать (80/20)

- Embedding = вектор; similarity search ≠ keyword search
- Индексы ANN (HNSW и др.) — приближённые; trade-off recall/latency
- Chunking, metadata filters, hybrid search (vector + keyword)
- Где жить: pgvector vs Pinecone/Qdrant/Weaviate/Milvus
- Стоимость: генерация embeddings, хранение, re-index при смене модели

## Дочерние узлы

Запланировано: pgvector, dedicated-vector-db, hybrid-search.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| pgvector vs dedicated vector DB | Один ops-стек vs спец. масштаб и фичи |
| Embed on write vs on query | Cost/latency записи vs свежесть при смене модели |

## Связанные узлы

- Postgres: [relational/postgres](../relational/postgres/)
- Extensions (pgvector): [relational/postgres/extensions](../relational/postgres/extensions/)
- AI-фичи: [07-product-adjacent/ai-features](../../07-product-adjacent/ai-features/)
