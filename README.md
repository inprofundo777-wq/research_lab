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
└── README.md
