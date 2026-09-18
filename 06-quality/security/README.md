# Security

> Актуальность: сентябрь 2026

## Роль в системе

Снижение риска компрометации и утечек: угрозы, поверхность атаки, контроли. Security — свойство дизайна и процесса поставки.

## Что нужно знать (80/20)

- STRIDE/базовая threat model на фичу
- OWASP-риски веб: injection, XSS, CSRF, broken auth, SSRF (на уровне решений)
- Secrets management; least privilege IAM
- Dependency и image scanning (см. supply-chain)
- Data protection: encryption in transit/at rest, PII minimization
- Secure defaults в фреймворках важнее самописного crypto

## Дочерние узлы

Запланировано: threat-modeling, app-security, secrets, compliance.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Build security in vs bolt-on audit | Дешевле на дизайне vs «проверим перед релизом» |
| WAF as primary vs fix root cause | Быстрый щит vs устранение уязвимости в коде |

## Связанные узлы

- Auth: [02-backend/auth](../../02-backend/auth/)
- Sessions / JWT: [02-backend/auth/sessions](../../02-backend/auth/sessions/), [02-backend/auth/jwt](../../02-backend/auth/jwt/)
- Supply chain: [05-cicd/supply-chain](../../05-cicd/supply-chain/)
- Browser platform: [01-frontend/browser-platform](../../01-frontend/browser-platform/)
