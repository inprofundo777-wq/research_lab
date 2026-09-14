# RR-RL-001 — Research Lab Role Architecture Review

## Паспорт

| Поле | Значение |
|---|---|
| **Document ID** | `RR-RL-001` |
| **Название** | Research Lab Role Architecture Review |
| **Статус** | `Final Analytical Review / Owner Confirmed` |
| **Дата** | 14.09.2026 |
| **Подготовил** | Project Overview |
| **Предмет** | Ролевая, процессная и документальная архитектура Research Lab |
| **Основание** | Архитектурный брейншторм Owner + Project Overview |
| **Текущий эффект** | Утверждённое аналитическое основание; само по себе не изменяет действующую Research Lab |
| **Решение Owner** | Архитектура и состав подтверждены 14.09.2026 |
| **Следующий шаг** | Repository Audit → Separate Change Set → Owner Pre-Write Review |

## Канонический контекст

- [Research Lab README](https://github.com/inprofundo777-wq/research_lab/blob/main/README.md)
- [Research Lab Constitution v0.2](https://github.com/inprofundo777-wq/research_lab/blob/main/Constitution/Constitution_v0.2.md)
- [Research Lab Methodology v0.3](https://github.com/inprofundo777-wq/research_lab/blob/main/Methodology/methodology_v0.3.md)
- [Research Lab Development](https://github.com/inprofundo777-wq/research_lab/blob/main/DEVELOPMENT.md)
- [IP-001 README](https://github.com/inprofundo777-wq/research_lab/blob/main/Research/IP-001/README.md)
- [IP-001 Protocol v0.2](https://github.com/inprofundo777-wq/research_lab/blob/main/Research/IP-001/IP-001_Protocol_v0.2.md)
- [IP-001 Primary Observation Output Contract v0.2](https://github.com/inprofundo777-wq/research_lab/blob/main/Research/IP-001/IP-001_Primary_Observation_Output_Contract_v0.2.md)

---

# 1. Executive Verdict

Research Lab уже обладает содержательным и методологическим основанием:

- Constitution;
- Methodology;
- проектом `IP-001`;
- Project Protocol;
- Stage architecture;
- Primary Observation Output Contract;
- опытом Romans controlled re-run;
- картой развития.

Однако лаборатория пока не обладает устойчивой системой ответственности, которая определяет:

- кто владеет всей Research Lab;
- кто принимает и формирует исследовательские запросы;
- кто проектирует отдельный Research Project;
- кто выполняет исследование;
- кто проводит независимую проверку;
- кто проводит Audit;
- кто управляет переходами и Close;
- как роли устанавливаются в новые ветки;
- как несколько активных версий ролей сосуществуют в параллельных исследованиях;
- как Research Result передаётся дальше без искажения.

Главный вывод Review:

> Перед полным возвращением к `IP-001` Research Lab нуждается в минимальной ролевой архитектуре из четырёх Core Roles, универсальной системе modes и пакетов A/B/C, двухуровневых картах проекта, независимом Audit и ступенчатой validation.

Архитектура подтверждена Owner и достаточно созрела для подготовки отдельного Change Set, но не для немедленного полного внедрения. До записи в GitHub требуется аудит действующей структуры репозитория и Owner Pre-Write Review цельного Change Set.

---

# 2. Основные архитектурные принципы

## 2.1. Research Before Application

Research Lab сохраняет установленную границу:

```text
Research
→ Synthesis
→ Architecture
→ Application
```

Предполагаемое применение может объяснять, почему возник Research Request, но не определяет, какой вывод исследование обязано получить.

## 2.2. Role, Mode и Package различаются

```text
Role
→ identity, authority, accountability

Mode
→ временная перспектива или capability

Package A / B / C
→ глубина установки контекста
```

Mode и Package не создают дополнительную authority.

## 2.3. Одна основная роль

Одна ветка может активировать несколько modes, но сохраняет одну Primary Role.

```text
One Primary Role
+ Optional Secondary Role
+ Multiple Active Modes
```

## 2.4. Автономия внутри управляющих документов

```text
Governing Documents
+ Current Source
+ Process Authority Envelope
+ Current Assignment
= автономное действие роли
```

При material conflict роль останавливается и передаёт минимальный upward output.

## 2.5. Независимость определяется процессом

Несколько перспектив одной ветки являются multi-perspective internal analysis, но не несколькими независимыми проверками.

Независимость требует отдельного прохода, отдельной ветки либо fresh judgment до сопоставления результатов.

## 2.6. Пропорциональная документация

Количество документов определяется объёмом и функцией работы, а не самим наличием стадии.

```text
Stage Complete
= required result produced
+ Output Contract satisfied
+ transition accepted
```

Один достаточный synthesis-файл может закрывать стадию. Большой объём может быть разделён на несколько файлов.

---

# 3. Ролевая пирамида

```text
Owner
→ Research Lab Director
→ Research Project Lead
→ Researcher
```

Research Auditor расположен сбоку от operational ownership и активируется по иерархии, Protocol или trigger.

## 3.1. Owner

Owner:

- определяет место Research Lab в In Profundo;
- подтверждает крупные новые Research Projects;
- утверждает изменения Constitution, постоянной authority и архитектуры;
- активирует Audit Research Lab Director;
- разрешает material conflict Director ↔ Auditor;
- принимает решения `ADOPT / TEST / REVISE / DEFER`.

## 3.2. Research Lab Director

Research Lab Director владеет всей Research Lab, а не отдельным проектом.

Он отвечает за:

- Research Horizon;
- диалог со Strategist;
- Research Request Map;
- Triage;
- интеллектуальную Orientation;
- карту существующих исследований;
- исторический, культурный, языковой, богословский и догматический контекст;
- формулирование Research Problem и Preliminary Research Question;
- определение предварительного corpus и масштаба;
- решение о маршруте запроса;
- назначение Research Project Lead;
- универсальную Role Library;
- развитие Methodology и Research capabilities;
- принятие Project Close Package;
- System Review и допустимость Knowledge Transfer.

Director не должен растворяться в одном Research Project.

## 3.3. Research Project Lead

Research Project Lead — универсальная роль, назначаемая на конкретный Research Project.

Он отвечает за:

- Project Installation;
- Project Charter;
- Protocol configuration;
- Stage architecture;
- Role Activation Matrix;
- Package A/B/C selection;
- Stage Assignments;
- Output Contracts;
- Verification Plan;
- Audit Gates;
- Project Map и Book Maps;
- структуру папок и документов;
- назначение Researcher;
- переходы между стадиями;
- operational Book Close;
- Project Close Package;
- возврат результата Director.

Lead проектирует способ исследования, но не переписывает интеллектуальное основание Director без возврата вопроса наверх.

## 3.4. Researcher

Researcher — универсальная рабочая роль.

Она:

- выполняет установленный Protocol;
- работает с назначенным corpus;
- различает Observation, Interpretation, Classification и Synthesis;
- сохраняет negative evidence;
- отмечает uncertainty;
- использует Stage Modes и Expert Modes;
- устанавливает verification flags;
- возвращает цельный output Project Lead;
- не меняет Research Question или scope самостоятельно;
- не выдаёт self-check за независимый Review.

## 3.5. Research Auditor

Research Auditor — независимая роль процессного и методологического контроля.

Он:

- проверяет соответствие Constitution, Methodology, Protocol и Output Contracts;
- проверяет traceability и воспроизводимость;
- проверяет пропорциональность вывода evidence;
- проверяет сохранность boundaries и independence;
- возвращает `PASS / PASS WITH CONDITIONS / RETURN / BLOCK / ESCALATE`;
- не переписывает проверяемую работу;
- не принимает project decision вместо Lead или Director.

---

# 4. Вход Research Request

## 4.1. Источники сигнала

Research opportunity может возникнуть из:

- Notion;
- Strategy Research Opportunity Portfolio;
- Content Portfolio;
- опубликованного корпуса;
- разговора Owner;
- комментариев Facebook или Telegram;
- повторяющихся вопросов аудитории;
- книги;
- существующего Research Project;
- внешнего исследования;
- актуального общественного или церковного вопроса;
- спонтанной идеи.

## 4.2. Strategy Research Opportunity Portfolio

Strategist сохраняет потенциальные направления в собственном контуре.

Этот Portfolio отвечает на вопрос:

> Какие исследовательские возможности видит проект?

Не каждая идея автоматически передаётся Research Lab.

## 4.3. Research Opportunity Package

При достаточном потенциале Strategist и Owner передают минимальный пакет:

- Request ID;
- источник сигнала;
- исследовательскую проблему;
- предварительный вопрос;
- актуальность;
- предполагаемое применение;
- Working Hypothesis, если существует;
- возможный scope;
- известные границы;
- ссылку на исходный Strategy artifact.

## 4.4. Research Request Map

Research Lab Director ведёт собственную карту официально переданных запросов.

Она отвечает на вопрос:

> Что передано Research Lab и что с этим происходит?

Цвета:

```text
⚪ received / not started
🟡 triage, formation or deferred
🟢 route determined or completed
🔴 blocked or out of scope
```

Цвет всегда сопровождается точным process status.

---

# 5. Formation и Project Installation

Для принятого запроса Director создаёт отдельный Formation-документ в Research Lab.

## 5.1. Director Formation

Director проводит:

- Triage;
- Existing Research Orientation;
- Historical Orientation;
- Cultural Orientation;
- Concept and Language Orientation;
- Exegetical Orientation;
- Theological/Dogmatic Orientation;
- position mapping;
- preliminary corpus design;
- assessment of project type and scale.

Не все проходы обязательны. Director включает их по необходимости.

Возможные результаты:

```text
NO RESEARCH REQUIRED
EXISTING RESEARCH PACKAGE
LIMITED RESEARCH REVIEW
LIMITED PROBE
FULL RESEARCH PROJECT
WATCH / DEFERRED
```

Точка передачи:

```text
ORIENTATION COMPLETE
→ READY FOR RESEARCH DESIGN
```

## 5.2. Project Installation

После Orientation Director назначает Project Lead.

Lead продолжает тот же Formation-документ и создаёт Installation Package:

- Research Project Charter;
- Research Question and Boundaries;
- corpus and sources;
- Stage Map;
- Role and Capability Matrix;
- inputs and outputs;
- Output Contracts;
- Verification Triggers;
- Audit Plan;
- document/folder architecture;
- decision authority;
- Stop Conditions;
- Close Criteria;
- Knowledge Transfer route.

## 5.3. Pre-Launch Audit

Перед запуском крупного или нового типа Research Project проводится единый Pre-Launch Audit:

- Orientation Audit;
- Installation Audit.

После Audit Director и, для material Full Project, Owner принимают Launch Decision.

---

# 6. Universal Researcher и Modes

## 6.1. Формула установки

```text
Researcher
= Core Identity
+ Stage Mode
+ Activated Expert Modes
+ Output Contract
```

## 6.2. Stage Modes

- Formation;
- Corpus Mapping;
- Primary Observation;
- Pattern Recognition;
- Classification;
- Synthesis;
- Knowledge Transfer.

## 6.3. Expert Modes

Кандидатный набор:

- Analytical;
- Exegetical;
- Greek Linguistic;
- Hebrew Linguistic;
- Historical;
- Cultural;
- Theological;
- Dogmatic;
- Canonical;
- Comparative;
- External Research Review.

Mode может работать под разными перспективами:

```text
Orientation
→ широкий контекст

Research
→ фокусное применение

Verification
→ проверка material claim

Synthesis
→ ограничение силы итогового вывода
```

## 6.4. Review как режим Researcher

Отдельная Core Role Research Reviewer пока не создаётся.

```text
Independent Research Review
= Researcher
+ fresh-context branch
+ Review Mode
+ Review Output Contract
```

Различаются:

- Independent Review — проверяет готовый output;
- Independent Re-check — сначала формирует собственный judgment, затем сравнивается с output.

---

# 7. Project Map и Book Map

## 7.1. Project Map

Одна компактная Project Map находится в папке Research Project.

Она показывает:

- список книг или research units;
- book-level maturity;
- активную книгу;
- следующий шаг;
- ссылку на Book Map;
- project-level stages отдельно от book-level status.

Состояния книги:

```text
⚪ not started
🟡 active
🟢 book-level closed
🔴 blocked
```

Зелёный статус книги не означает завершение cross-corpus synthesis.

## 7.2. Счётчик проекта

```text
Books: 27
Closed: N
Active: N
Awaiting Audit: N
Blocked: N
Not Started: N

Current Book: [Book]
Current Stage: [Stage]
Project-Level Synthesis: [Status]
```

Процент готовности не вычисляется автоматически, поскольку стадии имеют разный вес.

## 7.3. Book Map

Каждая книга получает компактную карту:

```text
Stage 0 — Book Corpus Map
Stage 1 — Primary Observation
Stage 2 — Repetition Mapping
Stage 3 — Provisional Classification
Verification Gate
Draft Stage 4 — Proposed Book Synthesis
Book-Level Close Audit
Final Book Close
```

Карта не перечисляет каждую главу.

## 7.4. Гранулярность документов

Stage 1 сохраняет установленную chapter-level документацию.

Обобщающие стадии могут использовать один или несколько документов в зависимости от объёма. Количество файлов не является показателем зрелости.

## 7.5. Book Cycle Document

Управляющий документ книги содержит:

- Passport;
- Book Process Map;
- Active Stage Assignment;
- Capability Configuration;
- Inputs;
- Output Contract;
- Verification and Audit Triggers;
- Stage Handoff;
- Output Index;
- Book Close.

Обычный Stage Assignment хранится внутри Book Cycle Document. Отдельный Assignment-файл создаётся только для сложной или многоветочной работы.

---

# 8. Audit Architecture

## 8.1. Гибридная активация

```text
Protocol / Trigger
→ AUDIT REQUIRED

Вышестоящая роль
→ назначает независимый Audit

Auditor
→ проводит проверку

Вышестоящая роль
→ принимает или эскалирует результат
```

## 8.2. Иерархия

| Что проверяется | Кто активирует |
|---|---|
| Researcher Output | Research Project Lead |
| Project Lead / Installation | Research Lab Director |
| Research Lab Director | Owner |
| Research Lab System | Owner |

## 8.3. Audit Modes

- Formation Audit;
- Installation Audit;
- Stage Audit;
- Book-Level Close Audit;
- Project Close Audit;
- System Audit.

## 8.4. Book-Level Close Audit

Правильное размещение:

```text
Stage 3
→ Verification Gate
→ Draft Stage 4 / Proposed Synthesis
→ Book-Level Close Audit
→ Final Book Close
```

Auditor должен видеть proposed synthesis, иначе он не может проверить пропорциональность итогового вывода.

## 8.5. Интенсивность

- Pre-Launch Audit — обязателен для крупного проекта или нового research type;
- Stage Audit — trigger-based;
- Book-Level Audit — обязателен перед Book Close;
- Project Close Audit — обязателен для крупного Research Project;
- System Audit — после полного проекта или достаточного повторяющегося evidence.

---

# 9. Authority и Upward Output

## 9.1. Иерархия документов

```text
In Profundo DNA
↓
Research Lab Constitution
↓
Research Lab Methodology
↓
Role Package
↓
Research Project Charter
↓
Project Protocol
↓
Stage Assignment
↓
Output Contract
```

Нижний документ конкретизирует работу, но не отменяет верхний.

## 9.2. Лестница решения

```text
Research Unit question
→ Researcher

Stage question
→ Research Project Lead

Project question
→ Research Lab Director

Lab / Structural question
→ Director / Owner
```

## 9.3. Эскалация

```text
Researcher
→ Project Lead
→ Research Lab Director
→ Owner
```

Перескок допустим при conflict of interest, нарушении independence, authority abuse, заблокированном маршруте или прямом запросе Owner.

## 9.4. Partial Stop

Эскалация получает один из режимов:

```text
CONTINUE LOCALLY
PARTIAL STOP
BLOCKED
```

Material вопрос одного passage не обязан останавливать всю книгу, если Protocol позволяет сохранить его unresolved.

## 9.5. Минимальный Result Contract

```markdown
# Research Handoff

**Status:** COMPLETE | BLOCKED | RETURN | ESCALATE
**Role:**
**Assignment:**
**Result / Decision:**
**Output:**
**Material findings:**
**Verification / Audit flags:**
**Boundary or conflict:**
**Capability Delta, if any:**
**Ownership returned to:**
**Next authorized step:**
**Open higher-level decision, if any:**
```

Upward output передаёт не всю рабочую историю, а Result, Boundary, Risk, Decision Needed и Next Step.

---

# 10. Role Installation и Recovery

## 10.1. One-link Installation

Новая ветка получает одну ссылку на активный Formation, Project, Book Cycle, Stage Assignment или Audit Assignment.

В документе находится Role Installation Block:

- Primary Role;
- Role Entry;
- Package A/B/C;
- Active Modes;
- Project / Stage;
- Protocol;
- Current Assignment;
- Output Contract;
- Process Authority Envelope;
- Return To.

## 10.2. Recovery Sequence

```text
Open Current Source
→ Read Role Installation Block
→ Open Role README
→ Load Package A/B/C
→ Load Active Modes
→ Read Protocol and Output Contract
→ Restore Authority
→ Check Conflicts
→ Declare Active Role
→ Begin Work
```

## 10.3. Recovery Stop

Работа не начинается, если отсутствуют:

- Role Entry;
- Package;
- Current Source;
- Protocol;
- scope;
- authority;
- Output Contract;
- Return Route.

## 10.4. Role Indicator

```text
▶ Основная роль — [Role]
▶ Основное задание — [Project / Stage]
■ Второстепенная роль — [inactive or Role]
◆ Активные моды — [Modes]
↔ Известные параллельные ветки — [State, if applicable]
```

---

# 11. Role Packages A/B/C

## 11.1. Package A — Minimal

Для узкой, повторяющейся и хорошо ограниченной задачи.

Содержит:

- identity;
- assignment;
- scope;
- Protocol section;
- Output Contract;
- authority;
- stop conditions;
- handoff.

## 11.2. Package B — Standard

Для обычной самостоятельной research work.

Package A плюс:

- Project Context;
- Thinking Framework;
- Stage Mode;
- Capability Configuration;
- verification triggers;
- relevant prior outputs;
- recovery instructions.

## 11.3. Package C — Extended

Для Formation, Installation, Synthesis, Audit, нового типа исследования или material conflict.

Package B плюс:

- Constitution;
- Methodology;
- Project Charter;
- Project Map;
- Decision Memory;
- cross-stage dependencies;
- extended verification;
- development history.

Package C не расширяет authority. Он только увеличивает глубину контекста.

---

# 12. Role Package Structure

## 12.1. Общий Role System Core

Кандидатный общий слой:

```text
Role_System/
├── README.md
├── Installation_Standard.md
├── Package_A-B-C.md
├── Mode_Standard.md
├── Authority_and_Escalation.md
├── Handoff_and_Result_Contracts.md
├── Independence_Boundary.md
└── Validation_Standard.md
```

## 12.2. Компактный пакет роли v0.1

Для первой версии не требуется сразу создавать полный набор документов Publication System.

Минимально:

```text
Roles/[Role]/
├── README.md
├── Charter.md
├── Operating_Model.md
└── Prompt.md
```

Потенциал роста закладывается через модульность. Thinking Framework, Workflow, Checklist, Decision Memory и Development выделяются позднее, если практика покажет, что компактный пакет перегружен.

## 12.3. Владение

Research Lab Director:

- создаёт и развивает universal Role Library;
- поддерживает A/B/C Standard;
- управляет universal modes;
- рассматривает Capability Gaps;
- организует Role Experiments;
- готовит material changes Owner.

Project Lead:

- выбирает роли и версии через Protocol;
- активирует modes;
- создаёт project-specific overlay;
- не переписывает universal Role Package;
- передаёт Capability Gap Director.

---

# 13. Multi-version Role Packages

## 13.1. Несколько активных версий

Несколько исследований могут использовать разные версии одной роли или mode.

```text
Researcher v0.1 — Supported
Researcher v0.2 — Default for New Work
Researcher v0.3 — Candidate
```

Canonical authority принадлежит Version Registry, а не одному постоянно перезаписываемому role-файлу.

## 13.2. Lifecycle

```text
CANDIDATE
ACTIVE
DEFAULT
SUPPORTED
DEPRECATED
RETIRED
ARCHIVED
```

## 13.3. Role Configuration Lock

Каждый Stage Assignment и Research Output фиксирует:

- Core Role version;
- Package A/B/C;
- Mode versions;
- Protocol version;
- Output Contract version;
- project overlay;
- installation date.

## 13.4. Adoption

Активный процесс выбирает:

```text
CONTINUE PINNED
ADOPT COMPATIBLE PATCH
MIGRATE AT STAGE BOUNDARY
MANDATORY MIGRATION
```

Новая версия не изменяет уже активные процессы автоматически.

## 13.5. Archive

Versioned paths желательно не перемещать физически после использования, чтобы не ломать ссылки из Research Outputs.

Архивирование происходит логически через статус Registry. Версия получает `ARCHIVED`, но остаётся доступной для воспроизводимости.

---

# 14. Role Evolution During Work

## 14.1. Уровни изменения

```text
Local Capability Delta
→ относится к одному assignment

Project Overlay
→ относится к одному проекту

Compatible Role Patch
→ универсальное совместимое уточнение

Role Revision
→ изменение identity, authority или обязательной архитектуры
```

## 14.2. Пропорциональное evidence

Небольшое исправление не должно ждать завершения всего `IP-001`. Материальное изменение не должно приниматься после одного неудобства.

## 14.3. Role Change Notice

Каждое изменение сообщает:

- Role;
- previous/new version;
- change class;
- reason;
- compatibility;
- effect on active processes;
- required action;
- validation status.

## 14.4. Универсальность

`Role Package Versioning and Evolution Standard` является кандидатом на общий стандарт In Profundo. Research Lab может стать его первой test implementation. Publication System не мигрирует автоматически.

---

# 15. Knowledge Transfer

## 15.1. Три уровня

```text
Research Result
≠ Knowledge Transfer Package
≠ Application Output
```

## 15.2. Ownership

- Director определяет допустимость и маршрут передачи;
- Project Lead готовит Transfer Package;
- Auditor проверяет material transfer по trigger;
- downstream owner решает, применять ли результат;
- downstream role создаёт книгу, статью, Portfolio или другой output.

## 15.3. Book-level Transfer

Допустим после Book-Level Audit и Final Book Close.

Он может утверждать только то, что подтверждено внутри конкретной книги.

```text
BOOK-LEVEL CLOSED RESULT
Cross-corpus conclusion not yet available
```

## 15.4. Project-level Transfer

Допустим после Cross-corpus Analysis, Project Close Audit и Final Synthesis.

Только здесь допустимы выводы уровня всего project corpus.

## 15.5. Transfer Routes

- Research → Strategist;
- Research → Book;
- Research → Editorial System;
- Research → New Research Request;
- Research → Public/Educational Output.

Application feedback возвращается как новый Research Signal, но не переписывает Research Result.

---

# 16. Validation Plan

Полный `IP-001` не должен быть первым общим тестом новой ролевой архитектуры.

## Wave 1 — Fresh-context Recovery

Проверить Director, Project Lead, Researcher и Auditor по одной ссылке.
