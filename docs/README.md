# Документация мода

Это первое проектное решение, не готовый игровой мод. Начинать с [этапов](roadmap.md), [требований](requirements.md) и [задач](../TASKS.md). Полное исходное видение сохранено в [first_prompt](../first_prompt), контекст работы — в [PROJECT.md](../PROJECT.md).

| Раздел | Материал |
| --- | --- |
| Видение и полнота | [Требования R-001–R-055](requirements.md), [связь с задачами](traceability.md), [этапы M0–M5](roadmap.md) |
| Архитектура | [Границы и владельцы состояния](architecture/overview.md), [контракты модулей](modules/contracts.md) |
| Игровая логика | [Специалисты](logic/specialists.md), [задачи и ревизии планов](logic/tasks_and_plans.md), [логистика и анализ фабрики](logic/logistics_and_analysis.md) |
| Система | [Совместимость клиентов](system/compatibility.md), [сохранения и разрушение](system/persistence.md), [интеграции мира](system/integration_matrix.md) |
| Управление и визуал | [Окно, пульт и планшет](system/interface.md), [игровые ассеты и переиспользование](system/assets_and_reuse.md) |
| Производительность | [Алгоритмы, бюджеты и локальные измерения](system/performance.md) |
| Проверки | [План QA/NET/PERF](testing/test_plan.md), [проверка первого решения](testing/planning_review.md) |
| Решения и материалы | [Варианты и вопросы владельцу](decisions.md), [первичные источники](research/sources.md) |

Слово «план» в TASKS означает работы по разработке. Внутриигровой план аналитика — отдельная сущность с UUID, revision и одобрением. Выполненные документы не закрывают игровые работы.
