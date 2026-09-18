# Patterns — паттерны React UI

> Актуальность: сентябрь 2026

## Роль в системе

Повторяемые способы оформить API компонента и поток данных: compound, controlled/uncontrolled API, headless. Архитектурно паттерн — контракт для потребителей дизайн-системы и фич, не коллекция сниппетов.

## Что нужно знать (80/20)

- Compound components: части (Trigger, Content) связаны через Context; снаружи — декларативное дерево
- Controlled vs uncontrolled API компонента: кто владеет open/value — родитель или внутренний state (часто оба режима)
- Headless / hooks-only: поведение и a11y без стилей; UI собирает потребитель
- Container/presentational — разделение wiring и разметки; полезно как идея границ, не как обязательные суффиксы
- State reducer / explicit state machine для сложных виджетов (меню, wizard) — предсказуемые переходы
- Избегать «паттерна ради паттерна»: если один prop достаточен — не тянуть compound
- Паттерн ≠ глобальный state management: см. слой [state](../../../state/) и [context](../context/)

## Дочерние узлы

Запланировано (без папок пока): детали compound/controlled как отдельные листья — только если эта карта перестанет влезать в один экран.

## Развилки

| Развилка | О чём спор (одна строка) |
| --- | --- |
| Compound vs плоские props | Гибкий слотовый API vs явный и простой контракт |
| Headless vs styled kit | Контроль дизайна vs скорость и единообразие |
| Свой виджет vs готовая библиотека | Fit продукта vs стоимость поддержки a11y/edge cases |

## Связанные узлы

- Родитель React: [../](../)
- Component: [../component/](../component/)
- Composition: [../component/composition/](../component/composition/)
- Controlled inputs: [../component/controlled-inputs/](../component/controlled-inputs/)
- Context: [../context/](../context/)
- Hooks: [../hooks/](../hooks/)
- UI: [../../../ui/](../../../ui/)
