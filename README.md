# In Profundo Research Lab

Research Lab — исследовательское направление In Profundo для дисциплинированного исследования Священного Писания.

Лаборатория отделяет исследование от последующей редакционной и публикационной работы:

> **Research → Synthesis → Architecture → Application**

Книги, статьи, курсы и другие материалы могут использовать результаты Research Lab, но не определяют их заранее.

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

### Конституция Research Lab

Определяет устойчивые принципы исследовательского направления.

Актуальная версия:

`Constitution/Constitution_v0.2.md`

### Методология Research Lab

Определяет общую эпистемическую дисциплину исследований независимо от конкретного Research Project.

Актуальная версия:

`Methodology/methodology_v0.3.md`

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
│   └── methodology_v0.3.md
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
├── Development/
├── Roles/
├── Processes/
└── README.md


---

# Role System v0.1

**Status:** 🟡 Implemented / Validation Pending

Core Roles:

- [Research Lab Director](./Roles/Director/v0.1/README.md)
- [Research Project Lead](./Roles/Project-Lead/v0.1/README.md)
- [Researcher](./Roles/Researcher/v0.1/README.md)
- [Research Auditor](./Roles/Auditor/v0.1/README.md)

All packages are Candidate Active and may be used only through staged validation. Their existence does not authorize a Full Research Project or IP-001 restart.

Formation begins only after explicit handoff:

~~~text
Strategist / Owner
→ Research Lab Director
→ Research Request Map
→ Formation
~~~

Far-horizon material remains potential until that handoff.
