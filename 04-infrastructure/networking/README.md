# Networking

> Актуальность: сентябрь 2026

## Роль в системе

Как трафик доходит до приложения: DNS, TLS, CDN, load balancing, private networks. Ошибки сети маскируются под «медленный бек».

## Что нужно знать (80/20)

- DNS, TLS-сертификаты, HTTP/2–3
- CDN и edge: кэш статики и иногда HTML/API
- Reverse proxy / load balancer; health checks
- Public vs private network; egress costs
- WAF, rate limiting на периметре (связь с security)
- Latency budget: географическое расстояние реально

## Дочерние узлы

Запланировано: dns-tls, cdn, load-balancing, private-networking.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Edge compute vs origin | Latency для пользователей vs сложность state/consistency |
| Terminate TLS at CDN vs origin | Упрощение origin vs end-to-end контроль |

## Связанные узлы

- Hosting: [hosting](../hosting/)
- Security: [06-quality/security](../../06-quality/security/)
- HTTP cache: [03-data/cache](../../03-data/cache/)
