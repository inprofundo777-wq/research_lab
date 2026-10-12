# IP-001 / Деяния — журнал книжного цикла и этапов

**Состояние:** Stage 0–2 приняты; следующий gate — Owner.  
**Паспорт:** [ACTS README](./README.md) · [проект IP-001](../../README.md).  
**Источник прежних решений:** [RL-WAVE-2 RUN, Events 039–064 и 071–072](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md).

Этот журнал группирует решения по этапам Деяний. Исторические решения ниже индексированы, а не приняты повторно.

| Этап | Действующая редакция | Решение | Открыто |
|---|---|---|---|
| Stage 0 — карта корпуса | [`rr-000…-R1`](./rr-000_Acts_Stage0_Corpus_Map-R1.md) | принята в историческом RUN | прежняя редакция сохранена |
| Stage 1 — первичные наблюдения | [`rr-001`](./rr-001_Acts_Primary_Observations.md) | [Event 060](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-060--project-lead-acceptance-acts-rr-stage-1-primary-observation) | вопросы Verification перенесены |
| Stage 2 — карта повторений | [`rr-002…-R1`](./rr-002_Acts_Repetition_Stable_Evidence_Map-R1.md) | [Event 072 — ACCEPT](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-072--ip-001-acts-rr-lead-focused-re-check-r1--accept-stage-2) | V01, V03, V04, V05, V10, V11, V12, V13, V14, V18 + O03 |
| Stage 3 | нет | не активирован | требуется отдельное решение Owner |
| Verification / Stage 4 / книжное закрытие | нет | не активированы | предметная проверка и независимый Book-Level Close Audit имеют отдельные зависимости |

## ACTS-D001 — навигационный перенос после Stage 2

**Дата:** 09.10.2026. **Основание:** [RL-D001](../../../../DECISIONS.md#rl-d001--решение-owner-о-языке-и-навигации) и [Event 072](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-072--ip-001-acts-rr-lead-focused-re-check-r1--accept-stage-2).

README Деяний синхронизирован с принятыми Stage 0–2. Это запись о навигации, не исследовательский вывод и не новое решение о приёмке. Исходные `doc-*`, `research-000.md`, `Summary.md`, `Book.md` и первоначальная `rr-002` сохраняются как история. Историческое сравнение по-прежнему запрещено до отдельного gate.

**Следующий owner:** Owner. **Следующий шаг:** отдельное решение о Stage 3 или другом ограниченном маршруте.


---

## ACTS-D002 — подготовка задания Stage 3; исполнение не разрешено

**Дата:** 12.10.2026. **Исполнитель:** Research Project Lead v0.1; Package C; bounded Installation only.  
**Источник полномочий:** прямое поручение Owner в действующей ветке Lead: «Подготовь Stage 3 для дальнейшей работы». Это поручение на подготовку, не execution authorization.  
**Target:** [ACTS-S3-PACK-v0.1 — пакет задания и договор ACTS-S3-OC-v0.1](https://github.com/inprofundo777-wq/research_lab/blob/8b680f9f05793a47ca88e7dc18075dc7475e87bf/Research/IP-001/Planning/ACTS-Stage-3-Assignment-Package-v0.1.md).

Подготовлены цельное задание Researcher, минимальный договор результата, точные принятые inputs, границы классификации, перенос 11 открытых Verification issues, критерии Lead acceptance, STOP/return, последующий fresh snapshot и текст предлагаемого Owner decision. Предварительные группы и rr-003 не создавались.

Для нового назначения явно закреплена Methodology v0.4; Protocol IP-001 v0.2 совместим с её языковым уточнением и сохраняет процедуру Stage 3. Прежние принятые результаты и их version pins не меняются. Package C выбран для Installation и предложен исполнителю из-за классификации с существенной неопределённостью, без расширения полномочий.

**Capability boundary:** Classification не входит в общий Scoped Active envelope Researcher v0.1. Пакет предлагает явное Owner-разрешение только контролируемого применения в этом Stage 3 с последующей проверкой handoff Lead; не объявляет режим в целом валидированным и не изменяет Registry.

**Внутренняя проверка:** требования пакета соотнесены с Protocol, Installation R1, Stage 2 R1 и новым правилом журналов; это self-check, не независимый Audit. Исторические Acts outputs и отклонённая карта Event 054 не открывались; RQ-RL-002 не затронут. Верхний historical RUN не обновляется: действует переход по RL-D001.

**Состояние:** STAGE 3 PREPARED / OWNER GATE / EXECUTION NOT AUTHORIZED. Stage 0–2 остаются принятыми; открытые вопросы не разрешены.  
**Ownership returned to Owner.**  
**Следующий шаг:** Owner утверждает конкретную редакцию пакета и отдельно разрешает ограниченное исполнение либо возвращает/откладывает его. После такого решения задание передаётся рабочей ветке Researcher IP-001; эта ветка Lead получает будущий handoff для приёмки. Подготовка не активирует Researcher, Stage 3, Material Verification, historical comparison, Stage 4 или независимые проверки.

Паспорта Деяний и IP-001 синхронизируются с этой подготовкой; проектный журнал содержит ссылку на данное решение, не дублирует договор.
