# Identity — продуктовая идентичность

> Актуальность: сентябрь 2026

## Роль в системе

Кто пользователь продукта: регистрация, SSO, MFA, social login, org/tenants. **Продуктовый** слой IdP; механики сессий/JWT на API — канон в [02-backend/auth](../../02-backend/auth/).

## Что нужно знать (80/20)

- Hosted IdP (Auth0, Clerk, Cognito, Keycloak, …) vs самопис
- OIDC для login; SCIM/приглашения для организаций
- MFA, passkeys — ожидание 2026 для серьёзных продуктов
- Модель пользователя vs организация/workspace
- Миграция пользователей и паролей — дорогой проект

## Дочерние узлы

Запланировано: hosted-idp, sso, mfa-passkeys, organizations.

Механики API — канонически в [02-backend/auth](../../02-backend/auth/): [sessions](../../02-backend/auth/sessions/), [jwt](../../02-backend/auth/jwt/), [oauth-oidc](../../02-backend/auth/oauth-oidc/), [rbac-abac](../../02-backend/auth/rbac-abac/).

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Hosted IdP vs self-host Keycloak | Скорость и фичи vs data residency и cost at scale |
| User-centric vs org-centric model | B2C простота vs B2B permissions |

## Связанные узлы

- Канон API auth: [02-backend/auth](../../02-backend/auth/)
- OAuth/OIDC: [02-backend/auth/oauth-oidc](../../02-backend/auth/oauth-oidc/)
- RBAC/ABAC: [02-backend/auth/rbac-abac](../../02-backend/auth/rbac-abac/)
- Security: [06-quality/security](../../06-quality/security/)
