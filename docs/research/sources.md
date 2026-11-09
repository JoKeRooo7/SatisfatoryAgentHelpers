# Источники и границы проверки

Дата обращения: 2026-11-09. Использованы первичные документы SML и Unreal. Сторонний код и игровые модели в ветку не включались. Теоретические проектные решения отдельно отмечены в спецификациях.

| Источник | Что подтверждает | Чего не подтверждает |
| --- | --- | --- |
| [SML: Required Software](https://docs.ficsit.app/satisfactory-modding/latest/Development/BeginnersGuide/dependencies.html) | Для моддинга нужна соответствующая игре модифицированная CSS-сборка Unreal и согласованная среда | Версию уже установленной у пользователя игры |
| [SML: Project Setup](https://docs.ficsit.app/satisfactory-modding/v3.11.3/Development/BeginnersGuide/project_setup.html) | Подготовка Starter Project и привязанных инструментов | Что номера из этой версии документации подходят любой новой игре |
| [SML: Releasing A Mod](https://docs.ficsit.app/satisfactory-modding/latest/Development/BeginnersGuide/ReleaseMod.html) | Поля совместимости модов, варианты сборки и проверки | Доставку модовых классов клиенту при выключенном требовании установки |
| [SML: Multiplayer](https://docs.ficsit.app/satisfactory-modding/latest/Development/Satisfactory/Multiplayer.html) | Authority, RCO, сетевое владение и необходимость проверки своего изменения мира | Рабочее подключение vanilla клиента к нашему ещё не написанному моду |
| [SML: Mod Subsystems](https://docs.ficsit.app/satisfactory-modding/latest/Development/ModLoader/Subsystems.html) | Варианты существования/репликации подсистем | Безопасность репликации модового класса отсутствующему клиенту |
| [SML: переход 3.7 → 3.8](https://docs.ficsit.app/satisfactory-modding/latest/Development/UpdatingFromSml37.html) | Историческое ограничение обратного подключения vanilla→SML | Текущую неизменность этого ограничения в установленной версии |
| [SML: переход 3.11 → 3.12](https://docs.ficsit.app/satisfactory-modding/latest/Development/UpdatingFromSml311.html) | Изменения среды для следующей связки; на странице есть предупреждение о невыпущенной поддержке | Что 3.12/1.2 уже следует выбирать стабильной средой проекта |
| [SML: Save Game](https://docs.ficsit.app/satisfactory-modding/latest/Development/Satisfactory/Savegame.html) | Интерфейсы и особенности включения состояния в сохранение | Общую транзакцию между любыми объектами и crash-proof запись каждого движения |
| [SML: FAQ](https://docs.ficsit.app/satisfactory-modding/latest/faq.html) | Категории multiplayer-модов и последствия загрузки без модового контента | Отсутствие конфликтов со всеми сторонними модами |
| [SML: Reusing Base Game Files](https://docs.ficsit.app/satisfactory-modding/latest/Development/ReuseGameFiles.html) | Использование игровых ассетов через runtime-ссылки/placeholder подход | Право включить извлечённые модели/шрифты в отдельный продукт |
| [SML: Extracting Game Files](https://docs.ficsit.app/satisfactory-modding/latest/Development/ExtractGameFiles.html) | Различие просмотра/извлечения и распространения защищённых файлов | Разрешение перепубликовывать файлы игры |
| [Unreal: SWindow](https://dev.epicgames.com/documentation/unreal-engine/API/Runtime/SlateCore/SWindow) | Наличие нативного оконного типа | Его пригодность во всех packaged сборках Satisfactory |
| [Unreal: FSlateApplication](https://dev.epicgames.com/documentation/unreal-engine/API/Runtime/Slate/FSlateApplication) | Инструменты окон/ввода Slate | Подтверждённые фокус/DPI/fullscreen сценарии нашего мода |
| [Unreal: Behavior Tree overview](https://dev.epicgames.com/documentation/unreal-engine/behavior-tree-in-unreal-engine---overview) | Событийный подход к поведению и возможности встроенного инструмента | Готовую навигацию и crafting/combat интеграцию NPC в игре |

Часть страниц `latest` показывает одновременно предупреждения dev/outdated. Поэтому ни одна конкретная версия SDK не зафиксирована только на основании этого адреса. В M0 требуется записать опубликованный release/tag, версии игры, SML, CSS Unreal, Starter Project, Wwise и Alpakit. Историческая заметка не заменяет эксперимент; недоступность исходного handshake при обращении отмечена в совместимости.

Практические материалы по стилю/ассетам находятся в [assets_and_reuse.md](../system/assets_and_reuse.md), по профилированию — в [performance.md](../system/performance.md). Источник правил процесса: [AIRules@8b74e311fec80a24d956e736174c7ae9aeec4fb0](https://github.com/JoKeRooo7/AIRules/tree/8b74e311fec80a24d956e736174c7ae9aeec4fb0).
