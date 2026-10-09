# In Profundo Research Lab

Research Lab — исследовательское направление In Profundo для дисциплинированного исследования Священного Писания.

Лаборатория отделяет исследование от последующей редакционной и публикационной работы:

> **Research → Synthesis → Architecture → Application**

Книги, статьи, курсы и другие материалы могут использовать результаты Research Lab, но не определяют их заранее.

---

## Быстрый вход: что действует сейчас

**Сверено:** 09.10.2026. [Журнал решений лаборатории](./DECISIONS.md) · [Правило навигации и журналов](./Processes/Documentation_and_Decision_Records.md).

| Объект | Состояние | Куда идти |
|---|---|---|
| [IP-001 — действия воскресшего Христа](./Research/IP-001/README.md) | исследование действует; в Деяниях Stage 0–2 приняты, следующий шаг решает Owner | [паспорт Деяний](./Research/IP-001/Research/ACTS/README.md), [журнал IP-001](./Research/IP-001/DECISIONS.md) |
| [RQ-RL-002 — сопровождение депрессии и суицидального кризиса](./Processes/Research_Request_Map.md) | Formation завершена; проект ограниченного обзора подготовлен, исполнение не разрешено | [Formation R2](./Development/Formations/FP-RL-002-Formation-Report-R2.md), [Installation Package](./Development/Validation-Runs/RL-WAVE-2/Artifacts/RQ-RL-002-Limited-Review-Installation-Package-v0.1.md) |

Запрос `RQ-RL-002` ещё не является `IP-002`: каталог нового исследования создаётся после соответствующего решения о запуске. Исторические решения Events 001–072 доступны в [RL-WAVE-2/RUN.md](./Development/Validation-Runs/RL-WAVE-2/RUN.md); его устаревшая верхняя сводка не заменяет последние полномочные Events. Текущая навигация живёт в README и журналах соответствующего уровня.

**Язык:** русский — единственный смысловой язык Research Lab на данном этапе по [Методологии v0.4](./Methodology/methodology_v0.4.md) §1.1. Коды, имена файлов, формальные статусы и цитаты источников могут сохранять исходный язык с русским объяснением.

---

## Архитектура документов

Research Lab работает внутри следующей структуры наследования:

> **DNA In Profundo**  
> ↓  
> **Конституция Research Lab**  
> ↓  
> **Методология Research Lab**  
> ↓  
> **Protocol конкретного Research Project**  
> ↓  
> **Stage-specific Output Contract**  
> ↓  
> **Research Output**

### DNA In Profundo

Определяет фундаментальную природу и основания всего проекта In Profundo.

Актуальная точка входа: [DNA In Profundo](https://github.com/inprofundo777-wq/editorial_system/blob/main/Constitution/DNA.md)

### Конституция Research Lab

Определяет устойчивые принципы исследовательского направления.

Актуальная версия:

`Constitution/Constitution_v0.2.md`

### Методология Research Lab

Определяет общую эпистемическую дисциплину исследований независимо от конкретного Research Project.

Актуальная версия:

[Методология v0.4](./Methodology/methodology_v0.4.md)

### Research Project Protocol

Определяет, как общая Methodology применяется к конкретному исследовательскому вопросу, corpus и процедуре исследования.

### Output Contract

Определяет минимальные требования к результату конкретной исследовательской стадии там, где отдельный контракт действительно необходим.

### Research Output

Содержит фактическое evidence, observations, Research Judgments, classifications и последующий synthesis.

### Role System

Role System является operational execution layer. Он определяет, какая роль, версия, Package, modes, Assignment и return route действуют внутри установленной иерархии.

Role System не изменяет epistemic authority Constitution, Methodology, Project Protocol или Output Contract.

Актуальная точка входа:

[Roles/README.md](./Roles/README.md)

Актуальные process surfaces:

- [Research Request Map](./Processes/Research_Request_Map.md)
- [Formation](./Processes/Formation/README.md)
- [Process Templates](./Processes/Templates/)
- [Навигация и журналы решений](./Processes/Documentation_and_Decision_Records.md)

---

# Структура репозитория

```text
research_lab/
│
├── Constitution/
│   ├── Constitution_v0.1.md
│   └── Constitution_v0.2.md
│
├── Methodology/
│   ├── methodology_v0.1.md
│   ├── methodology_v0.2.md
│   ├── methodology_v0.3.md
│   └── methodology_v0.4.md
│
├── Research/
│   │
│   └── IP-001/
│       │
│       ├── README.md
│       │
│       ├── IP-001_Protocol_v0.1.md
│       ├── IP-001_Protocol_v0.2.md
│       │
│       ├── IP-001_Primary_Observation_Output_Contract_v0.1.md
│       ├── IP-001_Primary_Observation_Output_Contract_v0.2.md
│       │
│       ├── Planning/
│       ├── Pilots/
│       ├── Research/
│       ├── Cross-analysis/
│       ├── Review/
│       ├── Final/
│       └── Archive/
│
├── DECISIONS.md
├── Development/
├── Roles/
├── Processes/
└── README.md


---

# Role System v0.1

**Status:** 🟡 Scoped Active in defined uses / broader modes Validation Pending

Core Roles:

- [Research Lab Director](./Roles/Director/v0.1/README.md)
- [Research Project Lead](./Roles/Project-Lead/v0.1/README.md)
- [Researcher](./Roles/Researcher/v0.1/README.md)
- [Research Auditor](./Roles/Auditor/v0.1/README.md)

Четыре роли v0.1 имеют статус **Scoped Active** только в точных областях, перечисленных в [Version Registry](./Roles/VERSION_REGISTRY.md). Все остальные режимы остаются **Validation Pending**.

Этот статус не разрешает автоматически Full Research Project, новый corpus или перезапуск IP-001. Для каждого процесса по-прежнему нужны установленная конфигурация и соответствующий Owner gate.

Formation begins only after explicit handoff:

~~~text
Strategist / Owner
→ Research Lab Director
→ Research Request Map
→ Formation
~~~

Far-horizon material remains potential until that handoff.
