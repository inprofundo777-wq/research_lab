# IP-001 — журнал решений проекта

**Исследовательский вопрос:** какие действия Новый Завет непосредственно приписывает воскресшему Иисусу Христу после Его Вознесения?  
**Состояние:** Деяния Stage 0–3 приняты; snapshot закреплён; P0 принят, C0 не готов/не разрешён; assessor/source gaps возвращены Owner.  
**Навигация:** [паспорт проекта](./README.md) · [Деяния](./Research/ACTS/README.md) · [журнал этапов Деяний](./Research/ACTS/DECISIONS.md)

## Исторические решения до перехода

| Область | Решение | Источник |
|---|---|---|
| Деяния: Installation | исправленный книжный цикл и отдельные зависимости проверки | [Events 045–048](../../Development/Validation-Runs/RL-WAVE-2/RUN.md) |
| Stage 0 | карта корпуса R1 принята | [RUN: Stage 0](../../Development/Validation-Runs/RL-WAVE-2/RUN.md) и [карта](./Research/ACTS/rr-000_Acts_Stage0_Corpus_Map-R1.md) |
| Stage 1 | первичные наблюдения приняты | [Event 060](../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-060--project-lead-acceptance-acts-rr-stage-1-primary-observation) и [наблюдения](./Research/ACTS/rr-001_Acts_Primary_Observations.md) |
| Stage 2 | русская редакция R1 принята; вопросы Verification открыты | [Event 072](../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-072--ip-001-acts-rr-lead-focused-re-check-r1--accept-stage-2) и [карта повторений](./Research/ACTS/rr-002_Acts_Repetition_Stable_Evidence_Map-R1.md) |

Точные решения и статус каждого этапа приведены в историческом RUN и журнале книжного цикла; эта таблица — навигация, не повторная приёмка.

## IP-001-D001 — переход на уровневую навигацию

**Дата:** 09.10.2026. **Основание:** решение Owner [RL-D001](../../DECISIONS.md#rl-d001--решение-owner-о-языке-и-навигации).  
README проекта и книжного цикла синхронизированы с Event 072. Применимая для новых назначений общая норма языка — [Методология v0.4](../../Methodology/methodology_v0.4.md); исторические назначения и принятые outputs сохраняют свою исходную version pin.

**Текущий gate:** Owner может отдельно назначить следующий ограниченный шаг; Stage 3, Material Verification, историческое сравнение и книжное закрытие не активированы. **Ownership — Owner.**


---

## IP-001-D002 — Stage 3 Деяний подготовлен; отдельный gate Owner

**Дата:** 12.10.2026. **Основание:** прямое поручение Owner подготовить дальнейший Stage 3.  
**Полная запись уровня этапа:** [ACTS-D002](./Research/ACTS/DECISIONS.md#acts-d002--подготовка-задания-stage-3-исполнение-не-разрешено).  
**Target:** [ACTS-S3-PACK-v0.1](https://github.com/inprofundo777-wq/research_lab/blob/8b680f9f05793a47ca88e7dc18075dc7475e87bf/Research/IP-001/Planning/ACTS-Stage-3-Assignment-Package-v0.1.md).

Lead подготовил задание, ACTS-S3-OC-v0.1, границы, критерии приёмки и предлагаемое Owner decision. Новое назначение использует Methodology v0.4 и Protocol v0.2; прежние результаты не переоткрыты. Ограниченное применение Classification Researcher v0.1 требует явного разрешения Owner; общий допуск режима не установлен.

**Проектное состояние:** Stage 0–2 приняты; Stage 3 подготовлен, но не активирован. **Ownership — Owner.** Следующее решение — утвердить/вернуть/отложить пакет и отдельно разрешить исполнение. Material Verification, историческое сравнение и книжное закрытие не активированы. Паспорт проекта и ближайший родительский паспорт Деяний синхронизированы.


---

## IP-001-D003 — Owner разрешил ограниченный Stage 3 Деяний

**Дата:** 12.10.2026. **Источник:** Owner «хорошо. утверждаю» в действующей ветке Lead.  
**Полное решение и назначение:** [ACTS-D003](./Research/ACTS/DECISIONS.md#acts-d003--решение-owner-разрешить-stage-3).

Утверждены ACTS-S3-PACK-v0.1 / ACTS-S3-OC-v0.1 в commit 8b680f9f05793a47ca88e7dc18075dc7475e87bf. Разрешено только контролируемое применение Classification к Stage 3 Деяний: Researcher v0.1, Package C; приёмка — действующая ветка Lead v0.1, Package C, Stage Coordination / Output Contract acceptance.

**Состояние:** Stage 3 AUTHORIZED / ACTIVE ASSIGNMENT; результат ещё не представлен/не принят. **Ownership:** Researcher → Lead → Owner. Общий допуск режима не изменён. Methodology v0.4 / Protocol v0.2 и границы Installation R1 закреплены; Stage 0–2 и открытые вопросы сохранены. Material Verification, историческое сравнение, Stage 4 и независимые проверки не разрешены.


---

## IP-001-D004 — Researcher представил Stage 3 Деяний

**Дата:** 12.10.2026. **Основание:** исполнение ACTS-D003 по утверждённому ACTS-S3-PACK-v0.1 / ACTS-S3-OC-v0.1.  
**Полный handoff:** [ACTS-D004](./Research/ACTS/DECISIONS.md#acts-d004--researcher-stage-3-представлен-для-приёмки-lead).  
**Target:** [rr-003 в commit 18b300ae11beeeccc483d75196fd3c9ca7914287](https://github.com/inprofundo777-wq/research_lab/blob/18b300ae11beeeccc483d75196fd3c9ca7914287/Research/IP-001/Research/ACTS/rr-003_Acts_Provisional_Groups.md).

Представлены четыре предварительные группы, сохранены 48 U/D/O, все R/S/NB/NM и 11 открытых вопросов. Внутренняя сверка не является независимой проверкой или acceptance. Прежние этапы не переоткрыты; исторические материалы не использованы.

**Состояние:** Stage 3 SUBMITTED / NOT ACCEPTED; **ownership — Lead для ACCEPT / RETURN → Owner**. Методологические и постоянные полномочия не изменены. Verification, историческое сравнение, Stage 4 и книжное закрытие не активированы. Паспорта проекта и Деяний синхронизированы; полный договор и исследовательское содержание не дублируются в этом журнале.


---

## IP-001-D005 — Lead принял Stage 3 Деяний

**Дата:** 12.10.2026. **Полное решение:** [ACTS-D005](./Research/ACTS/DECISIONS.md#acts-d005--lead-accept-stage-3-и-фиксация-fresh-snapshot); полномочия — ACTS-D003, handoff — ACTS-D004.

**ACCEPT STAGE 3.** Принят rr-003 в commit 18b300ae11beeeccc483d75196fd3c9ca7914287 как четыре предварительные группы, с охватом 48 ID, единичными и отрицательными основаниями и всеми 11 открытыми вопросами. Показана способность только к данному контролируемому применению Classification; постоянный Registry не изменён. Это internal Lead acceptance, не независимая Verification/Audit.

Зафиксирован [fresh Stage 0–3 snapshot](./Planning/ACTS-Fresh-Stage-0-3-Snapshot-2026-10-12.md) в commit 5936bf32a9ead62f200ac7b2c2b51a0f2781d6e5. **Деяния не закрыты как книга.** Сравнение с историческим материалом, Material Verification, Stage 4 и независимые проверки не активированы.

**Ownership returned to Owner.** Рекомендуемый следующий предмет подготовки — ограниченное назначение Material Verification с обеспечением capability/independence dependencies Installation R1; требуется отдельное Owner decision. Паспорта проекта и корпуса синхронизированы. Корневая навигация лаборатории остаётся долгом Director, указанным в ACTS-D005.


---

## IP-001-D006 — подготовлен пакет Material Verification Деяний

**Дата:** 12.10.2026. **Полная запись:** [ACTS-D006](./Research/ACTS/DECISIONS.md#acts-d006--lead-ограниченный-пакет-material-verification-представлен-owner).  
**Основание:** прямое Owner-поручение после ACTS-D005 подготовить проверку, не запускать её.  
**Target:** [ACTS-MV-PACK-v0.1](https://github.com/inprofundo777-wq/research_lab/blob/784283ed583f198302bc21cebb50d7f400b03afb/Research/IP-001/Planning/ACTS-Material-Verification-Package-v0.1.md).

Подготовлены матрица 11 вопросов (2 влияние на G03; 5 потенциальных изменений категории/субъекта/единичного основания; 4 потенциальных отдельных действия), порядок, точные договоры и отдельная capability проба на U04/U12/D20. Контекстная, Greek/syntax и text-critical способности и независимость оцениваются отдельно; операционная приёмка Lead не заменяет предметную компетенцию. Рекомендован Gate A только для дизайна/способности, затем отдельный Gate B для MV по реально подтверждённому scope.

**Состояние:** Stage 0–3 и snapshot приняты; MV-пакет PREPARED / OWNER GATE; все 11 вопросов открыты. Capability execution, Material Verification, historical comparison, Stage 4 и книжное закрытие не разрешены. **Ownership — Owner.** Паспорта проекта/корпуса обновлены; прежние outputs не менялись.


---

## IP-001-D007 — проект MV утверждён; CV-конфигурация возвращена Owner

**Дата:** 12.10.2026. **Решение Owner:** [ACTS-D007](./Research/ACTS/DECISIONS.md#acts-d007--owner-проект-mv-утверждён-разрешена-только-подготовка-cv-конфигурации). **Полный handoff:** [ACTS-D008](./Research/ACTS/DECISIONS.md#acts-d008--lead-cv-конфигурация-и-сообщения-подготовлены-возврат-owner).  
**Подготовленный target:** [CV-ACTS-IV-01-CONFIG-v0.1](https://github.com/inprofundo777-wq/research_lab/blob/69374fb4a639d46db350ded46fe3cc73c2fb4cb0/Research/IP-001/Planning/CV-ACTS-IV-01-Configuration-and-Branch-Messages-v0.1.md).

MV-проект принят как дизайн, не execution authorization. Подготовлены отдельные назначения IV Candidate / IV Assessor, первичные inputs/договоры, основания допуска и готовые сообщения. Предметный допуск конкретного нового оценщика не установлен и не выдан названием роли.

**Ownership — Owner.** Ближайший предлагаемый шаг — разрешить только P0 eligibility/source readiness новым веткам, первой IV Assessor; при наличии проверяемого готового оценщика Owner может отдельно закрепить scope и разрешить C0. Capability/MV/Stage 4 не выполнены/не активированы. Stage 0–3 и snapshot сохранены. Паспорта проекта/корпуса обновлены.


---

## IP-001-D008 — разрешён только P0 двух независимых веток

**Дата:** 12.10.2026. **Полное Owner decision:** [ACTS-D009](./Research/ACTS/DECISIONS.md#acts-d009--owner-cv-конфигурация-утверждена-разрешён-только-p0).

Owner утвердил CV-ACTS-IV-01-CONFIG-v0.1 в commit 69374fb4a639d46db350ded46fe3cc73c2fb4cb0 и разрешил только recovery/independence/source readiness/existing competence evidence: сначала новая IV Assessor, затем другая новая IV Candidate, Researcher v0.1 / Package C. Чаты ещё не созданы в рамках этой Lead-ветки; фактическое выполнение не заявлено.

**Ownership P0 outputs:** соответствующие ветки → Lead для договорной сверки → Owner. Компетенция оценщика не признана автоматически. Capability C0, предметная оценка sample, Material Verification и Stage 4 не разрешены. READY не запускает следующий этап. Паспорта обновлены.


---

## IP-001-D009 — P0 принят, readiness gaps возвращены Owner

**Дата:** 13.10.2026. **Полное решение:** [ACTS-D013](./Research/ACTS/DECISIONS.md#acts-d013--lead-p0-принят-c0-не-готов-возврат-owner). **Immutable readiness target:** [Readiness Decision](https://github.com/inprofundo777-wq/research_lab/blob/4fb87de6c4de8e74d93e4e88185410061d7ba55c/Research/IP-001/Review/CV-ACTS-IV-01-Readiness-Decision-v0.1.md).

ACTS-D011/D012 приняты как полные P0 records, не как экспертный допуск. Candidate capability и Assessor CTX/LANG/TEXT admission NOT ESTABLISHED; source readiness LIMITED, TEXT local warrant BLOCKED. Организационное разделение/раскрытие контекста учтены; полный epistemic/source-blind статус не заявлен.

**Ownership — Owner.** P0 завершён; C0/MV не готовы и не разрешены. Рекомендуется отдельное решение о Director bounded route consultation по основанию оценщика/ресурсам; альтернативы — существующее evidence, иной оценщик/разделение доменов, DEFER. Полное подготовленное поручение Director записано в ACTS-D013 как неактивное предложение; после Owner authorization передаётся одной ссылкой. Два P0 не повторяются без нового основания. Review и project/corpus passports синхронизированы.
