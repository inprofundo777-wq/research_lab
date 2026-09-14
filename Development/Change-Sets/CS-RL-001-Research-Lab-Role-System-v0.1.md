# CS-RL-001 — Research Lab Role System v0.1

## Паспорт

| Поле | Значение |
|---|---|
| **Change Set ID** | `CS-RL-001` |
| **Основание** | `RR-RL-001 — Final Analytical Review / Owner Confirmed` |
| **Статус** | `Approved for Controlled Write / Implementation In Progress` |
| **Дата** | 14.09.2026 |
| **Подготовил** | Project Overview |
| **Репозиторий** | `inprofundo777-wq/research_lab` |
| **Цель** | Создать минимальный ролевой и процессный слой Research Lab без запуска полного IP-001 |
| **Write Authority** | Owner разрешил контролируемую запись Batch 0–6 14.09.2026 |
| **Следующий Gate** | Sequential Implementation → Read-Back → Handoff → Role Exit |
| **Convergence Verdict** | `RECONCILED WITH CONDITIONS` — условия интегрированы |

---

# 1. Executive Decision

Предлагается внедрить не полную ролевую систему, а минимальную реализацию `v0.1`, достаточную для:

- восстановления четырёх Core Roles из новой ветки;
- формирования одного реального Research Request;
- подготовки Project Installation Package;
- независимого Pre-Launch Audit;
- проверки Role Configuration Lock и Result Contract;
- получения evidence до расширения системы.

Change Set не запускает полный `IP-001`, не переписывает Constitution и Methodology и не объявляет новые роли validated.

---

# 2. Repository Audit

## 2.1. Что уже существует и сохраняется

В репозитории уже закреплены:

- `Constitution/Constitution_v0.2.md`;
- `Methodology/methodology_v0.3.md`;
- `README.md` с иерархией исследовательских документов;
- `DEVELOPMENT.md`;
- действующий пакет `Research/IP-001/`;
- `IP-001_Protocol_v0.2.md`;
- `IP-001_Primary_Observation_Output_Contract_v0.2.md`;
- исторические и protocol-normalized outputs IP-001.

Constitution и Methodology уже обеспечивают:

- приоритет evidence;
- пропорциональность conclusions;
- сохранение ambiguity и negative result;
- разделение Research и Application;
- traceability и recoverability;
- свободу Project Protocol выбирать процедурную форму.

Поэтому их изменение в `CS-RL-001` не требуется.

## 2.2. Чего сейчас нет

Поиск по действующему репозиторию не обнаружил постоянных документов для:

- Research Lab Director;
- Research Project Lead;
- универсального Researcher;
- Research Auditor;
- Role Installation;
- Role Package A/B/C;
- Role Configuration Lock;
- Research Request Map;
- Formation;
- multi-version Role Packages;
- отдельного Knowledge Transfer Contract.

## 2.3. Обнаруженный статусный конфликт

`DEVELOPMENT.md` сейчас одновременно утверждает:

- Research Lab — `🟢`;
- IP-001 готов к полному protocol-normalized исследованию.

После решения Owner это описание неполно. Foundation действительно зрелый, но operational role capability ещё отсутствует и не validated.

Корректное состояние после записи Change Set:

```text
Research Lab Foundation — 🟢
Role Architecture — 🟡 Owner Confirmed / Implementation Pending
Role System v0.1 — 🟡 Implemented / Validation Pending
IP-001 — 🟡 Preserved / Full Restart Not Authorized
```

---

# 3. Архитектурная граница

Ролевая система является execution layer, а не новым уровнем epistemic authority.

```text
DNA
→ Research Lab Constitution
→ Research Lab Methodology
→ Project Protocol
→ Stage Output Contract
→ Research Output

Role System
→ устанавливает, кто и в каких границах исполняет эту иерархию
```

Role Package не может отменять, расширять или переопределять Constitution, Methodology либо Project Protocol. Role System организует исполнение epistemic requirements, но не создаёт параллельный epistemic authority layer.

---

# 4. Предлагаемая структура

```text
research_lab/
├── README.md                                      [UPDATE]
├── DEVELOPMENT.md                                 [UPDATE]
│
├── Development/                                   [NEW]
│   ├── Role-Reviews/
│   │   └── RR-RL-001-Research-Lab-Role-Architecture-Review.md
│   └── Change-Sets/
│       └── CS-RL-001-Research-Lab-Role-System-v0.1.md
│
├── Roles/                                         [NEW]
│   ├── README.md
│   ├── VERSION_REGISTRY.md
│   ├── Standards/
│   │   ├── Installation_Standard_v0.1.md
│   │   ├── Authority_and_Escalation_v0.1.md
│   │   ├── Independence_and_Audit_v0.1.md
│   │   └── Versioning_and_Evolution_v0.1.md
│   ├── Director/v0.1/
│   │   ├── README.md
│   │   ├── Charter.md
│   │   ├── Operating_Model.md
│   │   └── Prompt.md
│   ├── Project-Lead/v0.1/
│   │   ├── README.md
│   │   ├── Charter.md
│   │   ├── Operating_Model.md
│   │   └── Prompt.md
│   ├── Researcher/v0.1/
│   │   ├── README.md
│   │   ├── Charter.md
│   │   ├── Operating_Model.md
│   │   └── Prompt.md
│   └── Auditor/v0.1/
│       ├── README.md
│       ├── Charter.md
│       ├── Operating_Model.md
│       └── Prompt.md
│
├── Processes/                                     [NEW]
│   ├── Research_Request_Map.md
│   ├── Formation/
│   │   ├── README.md
│   │   └── Formation_Template.md
│   └── Templates/
│       ├── Role_Configuration_Lock.md
│       ├── Project_Map.md
│       ├── Book_Cycle.md
│       └── Research_Handoff.md
│
├── Constitution/                                  [UNCHANGED]
├── Methodology/                                   [UNCHANGED]
└── Research/IP-001/                               [PRESERVED]
```

---

# 5. Содержание новых документов

## 5.1. `Roles/README.md`

Единая точка входа в Role System. Она должна:

- объяснять различие Role, Package, Mode и Process Function;
- показывать четыре Core Roles;
- направлять в Version Registry;
- определять Recovery Sequence;
- содержать обязательный Role Indicator;
- запрещать считать наличие пакета доказательством validation.

## 5.2. `Roles/VERSION_REGISTRY.md`

Единственный lab-level источник статуса версий.

Начальное состояние:

| Role | Version | Status | Default | Validation |
|---|---:|---|---|---|
| Research Lab Director | v0.1 | Candidate Active | yes | pending |
| Research Project Lead | v0.1 | Candidate Active | yes | pending |
| Researcher | v0.1 | Candidate Active | yes | pending |
| Research Auditor | v0.1 | Candidate Active | yes | pending |

`Candidate Active` означает: пакет разрешён только для validation work, но ещё не доказан устойчивой практикой.

## 5.3. Role Standards

### Installation Standard

Закрепляет:

- Packages A/B/C;
- одну Primary Role;
- optional Secondary Role;
- несколько совместимых modes;
- Role Configuration Lock;
- Recovery Stop;
- Result Contract и return route.

### Authority and Escalation

Закрепляет:

```text
Researcher → Project Lead → Director → Owner
```

и результаты эскалации:

```text
CONTINUE LOCALLY
PARTIAL STOP
BLOCKED
```

### Independence and Audit

Различает:

- internal multi-perspective analysis;
- Independent Review;
- Independent Re-check;
- Research Audit.

Также закрепляет иерархию назначения аудитора и конфликтный маршрут.

### Versioning and Evolution

Сначала хранится как Research Lab pilot-standard.

Он закрепляет:

- несколько одновременно активных версий;
- Version Registry как canonical authority;
- отсутствие скрытой миграции действующего процесса;
- `CONTINUE PINNED`, `ADOPT COMPATIBLE PATCH`, `MIGRATE AT STAGE BOUNDARY`, `MANDATORY MIGRATION`;
- логическое архивирование после прекращения использования версии всеми процессами.

Перенос стандарта на уровень всего In Profundo допускается только после validation.

## 5.4. Четыре Role Packages

Каждый пакет `v0.1` состоит только из четырёх документов:

| Документ | Функция |
|---|---|
| `README.md` | точка входа, Recovery и навигация |
| `Charter.md` | identity, purpose, authority, boundaries |
| `Operating_Model.md` | activation, work, handoff, exit, escalation |
| `Prompt.md` | компактная установка роли в новую ветку |

Отдельные Thinking Framework, Workflow, Checklist, Decision Memory и Development пока не создаются.

## 5.5. Modes

На первой версии modes не получают отдельный каталог файлов. Они описываются компактно внутри Operating Model соответствующей роли и вызываются через Assignment.

Минимальный набор:

- Director: `Formation / Wide Orientation`;
- Researcher: `External Research`, `Historical`, `Linguistic`;
- Auditor: `Formation Audit`, `Installation Audit`, `Methodological Audit`;
- Project Lead: `Installation`.

Выделение отдельного Mode Package допускается только после evidence, что встроенного описания недостаточно.

## 5.6. Research Request Map

Размещается в `Processes/Research_Request_Map.md`.

Карта учитывает только запросы, формально переданные в Research Lab. Strategy Research Opportunity Portfolio остаётся upstream-документом Strategist и не переносится в репозиторий Research Lab автоматически.

Статусы:

| Marker | Exact Status |
|---|---|
| ⚪ | RECEIVED / NOT STARTED |
| 🟡 | TRIAGE / FORMATION / DEFERRED |
| 🟢 | ROUTE DETERMINED / COMPLETED |
| 🔴 | BLOCKED / OUT OF SCOPE |

## 5.7. Formation

Один Formation Document содержит две последовательные зоны ownership:

```text
Director Formation / Orientation
→ Formation Decision
→ Project Lead Installation
→ Pre-Launch Audit
→ Launch Decision
```

Формация может завершиться без запуска Research Project.

Допустимые результаты:

- `NO RESEARCH REQUIRED`;
- `EXISTING RESEARCH PACKAGE`;
- `LIMITED REVIEW`;
- `LIMITED PROBE`;
- `FULL PROJECT`;
- `DEFERRED / WATCH`.

## 5.8. Maps и Handoff

- `Project_Map.md` — компактная карта книг/corpora и project-wide stages;
- `Book_Cycle.md` — Passport, Book Map, Active Assignment, Role Lock, outputs, audit и close;
- `Role_Configuration_Lock.md` — точная версия роли, Package, modes, Protocol, Output Contract и return route;
- `Research_Handoff.md` — Result, Evidence Boundary, Risk, Decision Needed, Next Step, Ownership Returned.

---

# 6. Изменения существующих документов

## 6.1. Root `README.md`

Добавить:

- Role System как execution layer;
- ссылки на `Roles/README.md`, Version Registry и Research Request Map;
- различие Strategy Opportunity Portfolio и Research Request Map;
- маршрут Formation;
- предупреждение: роли `v0.1` имеют статус Candidate Active.

Не изменять существующие epistemic определения.

## 6.2. `DEVELOPMENT.md`

Обновить состояние без удаления исторического evidence:

- Foundation оставить `🟢`;
- Research Lab operational capability перевести в `🟡 Role System Validation`;
- зафиксировать Owner-confirmed architecture;
- полный IP-001 не считать следующим автоматическим шагом;
- показать validation Waves 1–4 как ближайший горизонт;
- сохранить Romans controlled re-run как methodology evidence, но не как role validation.

## 6.3. `Research/IP-001/`

В `CS-RL-001` не изменять:

- Protocol;
- Output Contract;
- Research outputs;
- статусы книг;
- исторические материалы.

IP-001 используется только позднее и только в явно разрешённом validation scope.

---

# 7. Решения по Implementation Questions

| Вопрос | Решение Change Set |
|---|---|
| Первый Formation Pilot | Один реальный bounded far-horizon request из нового Portfolio после explicit handoff `Strategist / Owner → Research Lab Director`; Director не активирует Content Horizon самостоятельно |
| Strategy Research Opportunity Portfolio | Остаётся upstream у Strategist; Research Lab хранит только ссылку и принятый Request |
| Research Request Map | `Processes/Research_Request_Map.md` |
| Versioning Standard | Pilot в `Roles/Standards/`; общепроектное принятие только после validation |
| Минимальные modes | Formation, Installation, External Research, Historical, Linguistic, Formation/Installation/Methodological Audit |
| IP-001 для ранней validation | Romans outputs используются read-only для Recovery/Audit test; исследование не возобновляется |
| Future Book Cycle Pilot | Небольшая книга Нового Завета выбирается отдельным Owner gate после Waves 1–6 |
| Methodology | В v0.1 не изменяется; gap фиксируется как evidence для отдельной revision |

Первый Formation Pilot нельзя начать, пока Strategist и Owner не передали конкретный кандидатный запрос в Research Lab. Far Horizon остаётся пространством потенциала, а не списком автоматически активируемых Research Projects. Director формирует и оценивает принятый запрос, но не присваивает ownership Content Horizon. Отсутствие темы не блокирует создание ролевого слоя, но блокирует Wave 2.

---

# 8. Validation Route

## Wave 1 — Fresh-context Role Recovery

Для каждой из четырёх ролей:

- новая изолированная ветка;
- вход только через Role README;
- Package B;
- проверка identity, authority, boundaries, handoff и exit;
- отсутствие записи в Research outputs.

## Wave 2 — Formation Pilot

- один реальный Request;
- Director Orientation;
- при необходимости Researcher modes;
- Formation Audit;
- Formation Decision.

## Wave 3 — Installation Pilot

Только если Formation Decision требует исследования:

- Project Lead Installation;
- Protocol configuration;
- Project/Book Map selection;
- Role Configuration Lock;
- Pre-Launch Audit.

## Wave 4 — Micro Research Cycle

Один bounded unit. Не полный IP-001.

После каждой Wave:

```text
ADOPT
TEST FURTHER
REVISE
DEFER
```

Waves 5–9 остаются дальнейшим горизонтом и не входят в первую запись.

---

# 9. Implementation Batches

## Batch 0 — Preserve Decision

- записать `RR-RL-001`;
- записать финальный `CS-RL-001`;
- не изменять operational system.

## Batch 1 — Role System Core

- создать `Roles/README.md`;
- создать Version Registry;
- создать четыре Standards;
- повторно проверить ссылки и authority boundaries.

## Batch 2 — Core Role Packages

- создать четыре пакета `v0.1`;
- провести cross-role consistency check;
- не присваивать статус Validated.

## Batch 3 — Process Surfaces

- создать Research Request Map;
- создать Formation и четыре templates;
- проверить, что простые Assignment остаются внутри Book Cycle Document.

## Batch 4 — Navigation and Status

- обновить root README;
- обновить DEVELOPMENT;
- проверить все ссылки и статусы;
- завершить Post-Write Consistency Check.

## Batch 5 — Validation Preparation

- подготовить четыре Recovery assignments;
- не запускать Wave 2 без реального Request и отдельного Owner signal.

## Batch 6 — Temporary Role Exit and Project-Level Handoff

После завершения разрешённых записей Project Overview:

- передаёт operational ownership созданного пакета Research Lab Director;
- фиксирует, что роль Director остаётся Candidate и ещё не validated;
- выходит из временной функции `Research System Design`;
- выполняет Scale Recovery к общепроектной карте;
- сохраняет один material delta в `Project-Overview/Role_Activity_Log.md`;
- отдельно предлагает точечное обновление `Project_Map.md` и Development Map, не включая эти cross-repository изменения автоматически в `CS-RL-001`.

Этот Batch является первым реальным кандидатом на evidence для `DS-03 — Temporary-role document work`. Успешная запись документов сама по себе не закрывает DS-03: должны быть доказаны Handoff, Role Exit и Scale Recovery.

---

# 10. Migration and Rollback

## Migration Boundary

- существующие Research outputs сохраняют provenance;
- роли не применяются задним числом;
- IP-001 не переводится автоматически на новые пакеты;
- каждый новый process фиксирует точную Role Configuration;
- Publication System не мигрирует на этот standard автоматически.

## Rollback Boundary

Если v0.1 создаёт procedural burden или authority conflict:

- остановить новые activations;
- пометить Candidate versions как `DEPRECATED — VALIDATION FAILED`;
- сохранить файлы и evidence;
- вернуть operational authority к Constitution, Methodology и действующим Protocols;
- подготовить corrective Change Set.

Rollback не удаляет исторические файлы и не переписывает результаты исследований.

---

# 11. Explicit Non-Goals

В `CS-RL-001` не входят:

- полный запуск IP-001;
- создание IP-002;
- изменение Constitution;
- изменение Methodology;
- отдельная Core Role Research Reviewer;
- отдельные stage-specific researcher roles;
- полный каталог modes;
- обязательный аудит каждого Stage;
- автоматизация GitHub/оркестратор;
- перенос Research Result в книгу или публикацию;
- перестройка Publication System;
- общепроектное принятие Versioning Standard.

---

# 12. Pre-Write Checks

Перед любой записью необходимо:

1. признать завершённым Parallel Branch Convergence Check Project Overview с verdict `RECONCILED WITH CONDITIONS`;
2. проверить, что три условия Convergence встроены в финальную редакцию: maturity status отделён от Owner approval; Formation Pilot требует explicit Strategist/Owner handoff; Role System подчинён Constitution/Methodology;
3. повторно прочитать актуальные README, DEVELOPMENT, Constitution и Methodology;
4. проверить отсутствие новых конфликтующих файлов;
5. подтвердить точные пути и имена;
6. убедиться, что GitHub write operation разрешена Owner отдельно;
7. записывать последовательными batches с проверкой после каждого.

---

# 13. Owner Pre-Write Decisions Requested

Перед реализацией Owner предлагается подтвердить или скорректировать:

1. предложенную структуру каталогов;
2. четыре документа в каждом Role Package v0.1;
3. хранение modes внутри Operating Model на первой версии;
4. размещение Versioning Standard сначала в Research Lab;
5. размещение Research Request Map в `Processes/`;
6. отсутствие изменений Constitution и Methodology;
7. корректировку статуса `DEVELOPMENT.md`;
8. сохранение IP-001 без перезапуска;
9. Romans как read-only evidence для раннего Recovery/Audit test;
10. первый Formation Pilot из нового far-horizon Portfolio;
11. последовательность Batch 0–6, включая Temporary Role Exit и project-level handoff;
12. отдельный Owner write signal после завершённой межветочной сверки.

---

# 14. Parallel Branch Convergence Disposition

## Verdict

```text
RECONCILED WITH CONDITIONS
```

Архитектурных конфликтов с Research Lab Foundation, Project Overview boundaries или текущим project focus не обнаружено.

## Интегрированные условия

1. `Role Architecture` имеет статус `🟡 Owner Confirmed / Implementation Pending`, а не зелёную maturity-mark.
2. Первый far-horizon Formation Pilot запускается только через explicit handoff `Strategist / Owner → Research Lab Director`.
3. Role System явно остаётся operational layer ниже Constitution, Methodology и project-specific epistemic requirements.
4. Реализация через Project Overview завершается отдельными Handoff, Temporary Role Exit и Scale Recovery.

## Map Consequences

После реализации, но не до неё, требуется отдельная project-level операция:

- заменить устаревшее положение Project Map об отсутствии постоянной Research leadership;
- показать Research Lab Director → Research Project Lead → Researcher и independent Auditor компактно, без дублирования Role System;
- сохранить Foundation `🟢`;
- показать Role System `🟡 Validation Pending`;
- сохранить IP-001 `🟡 Preserved / Full Restart Not Authorized`;
- внести staged validation как ближайший переход, но не новый долгосрочный главный фокус;
- признать validation ролей новым evidence debt;
- не создавать новый Research Snapshot до material validation result.

Эти изменения не входят автоматически в write authority `CS-RL-001` и требуют собственного project_hub Change Set либо явно расширенного разрешения Owner.

## Readiness

После интеграции условий настоящий документ имеет verdict:

```text
READY FOR OWNER WRITE DECISION
```

## Утверждённый статус

```text
Approved for Controlled Write
```

Этот статус разрешает реализацию только описанных batches и не разрешает полный Research Project либо IP-001 restart. Решение Owner получено 14.09.2026.