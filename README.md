# Essential — справочник веб-архитектуры

> Актуальность карты: **сентябрь 2026**

Личный архитектурный справочник: зашёл в узел дерева — увидел, **что нужно понимать**, чтобы принимать решения. Не учебник и не полный курс. Принцип Парето: 80/20 основ и развилок по всем слоям веб-проекта.

## Зачем это

Цель — владеть **структурным** пониманием веб-проектов: фронт, бек, данные, инфраструктура, CI/CD, качество. Глубокая экспертиза в каждой технологии не требуется; требуется умение видеть слой, роль, развилку и цену усложнения.

## Как читать

1. Начни с [`00-system/`](00-system/) — путь запроса и модель слоёв.
2. Дальше — по дереву снизу: слой → подобласть → технология.
3. Каждый каталог открывается в `README.md` — карта узла (роль, 80/20, дочерние, развилки).
4. Правила оформления: [`CONVENTIONS.md`](CONVENTIONS.md).

## Чем проект не является

- Не курс «выучи React / Docker за N дней»
- Не awesome-list ссылок
- Не канонический «единственно верный» стек
- Пока без `GUIDE.md` и примеров-подпроектов (запланированы для листьев, где карта недостаточна)

## Дерево

```
essential/
├── 00-system/                 # Позвоночник: путь запроса, стили, качество
├── 01-frontend/               # Браузер, рендер, UI, state
├── 02-backend/                # Рантаймы, API, нарезка сервиса
├── 03-data/                   # Моделирование и хранилища
├── 04-infrastructure/         # Хостинг, сеть, контейнеры, облака
├── 05-cicd/                   # Pipeline, деплой, GitOps
├── 06-quality/                # Тесты, observability, security, reliability
└── 07-product-adjacent/       # Identity, payments, flags, AI-фичи
```

### Полное дерево со ссылками

- [`00-system/`](00-system/) — из чего состоит веб-проект
  - [`request-path/`](00-system/request-path/) — путь запроса от клиента до данных
  - [`architecture-styles/`](00-system/architecture-styles/) — monolith, modular monolith, microservices, …
  - [`quality-attributes/`](00-system/quality-attributes/) — latency, consistency, cost, complexity
- [`01-frontend/`](01-frontend/)
  - [`browser-platform/`](01-frontend/browser-platform/)
  - [`rendering/`](01-frontend/rendering/)
  - [`frameworks/`](01-frontend/frameworks/)
    - [`react/`](01-frontend/frameworks/react/)
      - [`component/`](01-frontend/frameworks/react/component/) ← эталонный лист
    - [`vue/`](01-frontend/frameworks/vue/)
    - [`angular/`](01-frontend/frameworks/angular/)
    - [`svelte/`](01-frontend/frameworks/svelte/)
    - [`solid/`](01-frontend/frameworks/solid/)
    - [`html-first/`](01-frontend/frameworks/html-first/)
  - [`meta-frameworks/`](01-frontend/meta-frameworks/)
    - [`nextjs/`](01-frontend/meta-frameworks/nextjs/)
  - [`ui/`](01-frontend/ui/)
  - [`state/`](01-frontend/state/)
  - [`data-fetching/`](01-frontend/data-fetching/)
  - [`styling/`](01-frontend/styling/)
  - [`performance/`](01-frontend/performance/)
  - [`accessibility/`](01-frontend/accessibility/)
- [`02-backend/`](02-backend/)
  - [`runtimes/`](02-backend/runtimes/)
  - [`frameworks/`](02-backend/frameworks/)
  - [`api-styles/`](02-backend/api-styles/)
    - [`rest/`](02-backend/api-styles/rest/)
    - [`graphql/`](02-backend/api-styles/graphql/)
    - [`rpc/`](02-backend/api-styles/rpc/)
  - [`service-boundaries/`](02-backend/service-boundaries/)
  - [`auth/`](02-backend/auth/)
    - [`sessions/`](02-backend/auth/sessions/)
    - [`jwt/`](02-backend/auth/jwt/)
    - [`oauth-oidc/`](02-backend/auth/oauth-oidc/)
    - [`rbac-abac/`](02-backend/auth/rbac-abac/)
  - [`async/`](02-backend/async/)
- [`03-data/`](03-data/)
  - [`modeling/`](03-data/modeling/)
  - [`relational/`](03-data/relational/)
    - [`postgres/`](03-data/relational/postgres/)
      - [`indexing/`](03-data/relational/postgres/indexing/)
      - [`replication/`](03-data/relational/postgres/replication/)
      - [`extensions/`](03-data/relational/postgres/extensions/)
  - [`document/`](03-data/document/)
  - [`cache/`](03-data/cache/)
  - [`search/`](03-data/search/)
  - [`analytics/`](03-data/analytics/)
  - [`vectors/`](03-data/vectors/)
  - [`data-access/`](03-data/data-access/)
    - [`orm-vs-sql/`](03-data/data-access/orm-vs-sql/)
    - [`migrations/`](03-data/data-access/migrations/)
    - [`transactions/`](03-data/data-access/transactions/)
- [`04-infrastructure/`](04-infrastructure/)
  - [`networking/`](04-infrastructure/networking/)
  - [`hosting/`](04-infrastructure/hosting/)
  - [`containers/`](04-infrastructure/containers/)
    - [`docker/`](04-infrastructure/containers/docker/)
      - [`dockerfile/`](04-infrastructure/containers/docker/dockerfile/)
      - [`compose/`](04-infrastructure/containers/docker/compose/)
  - [`orchestration/`](04-infrastructure/orchestration/)
  - [`iac/`](04-infrastructure/iac/)
  - [`environments/`](04-infrastructure/environments/)
  - [`clouds/`](04-infrastructure/clouds/)
- [`05-cicd/`](05-cicd/)
  - [`git-flow/`](05-cicd/git-flow/)
  - [`pipeline/`](05-cicd/pipeline/)
    - [`stages/`](05-cicd/pipeline/stages/)
  - [`platforms/`](05-cicd/platforms/)
    - [`github-actions/`](05-cicd/platforms/github-actions/)
  - [`preview-rollout/`](05-cicd/preview-rollout/)
  - [`gitops/`](05-cicd/gitops/)
  - [`supply-chain/`](05-cicd/supply-chain/)
- [`06-quality/`](06-quality/)
  - [`testing/`](06-quality/testing/)
  - [`observability/`](06-quality/observability/)
  - [`security/`](06-quality/security/)
  - [`reliability/`](06-quality/reliability/)
- [`07-product-adjacent/`](07-product-adjacent/)
  - [`identity/`](07-product-adjacent/identity/)
  - [`payments/`](07-product-adjacent/payments/)
  - [`notifications/`](07-product-adjacent/notifications/)
  - [`feature-flags/`](07-product-adjacent/feature-flags/)
  - [`ai-features/`](07-product-adjacent/ai-features/)

## Ориентиры индустрии (не истина)

На сентябрь 2026 часто встречаются как **дефолты**, а не как обязательный выбор:

| Слой | Частый ориентир |
| --- | --- |
| Frontend | React + мета-фреймворк (часто Next.js), TypeScript, Vite |
| Backend | Node/Nest или Python/FastAPI; modular monolith |
| Data | PostgreSQL как system of record, Redis рядом |
| Infra / CI | PaaS → контейнеры → k8s по необходимости; GitHub Actions |

См. развилки внутри каждого слоя — там карта альтернатив.

## Дальше

Трекинг наполнения: [`PROGRESS.md`](PROGRESS.md).

Когда карта узла перестанет хватать для архитектурного выбора — добавляй `GUIDE.md` и при необходимости `examples/` по правилам из [`CONVENTIONS.md`](CONVENTIONS.md).
