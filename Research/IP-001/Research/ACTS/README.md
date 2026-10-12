# IP-001 — Деяния апостолов

**Состояние:** свежий проход Stage 0–2 принят; Stage 3 подготовлен, исполнение не разрешено; следующий gate у Owner.  
**Сверено:** 12.10.2026 по [ACTS-D002](./DECISIONS.md#acts-d002--подготовка-задания-stage-3-исполнение-не-разрешено); приёмка Stage 2 — [Event 072](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-072--ip-001-acts-rr-lead-focused-re-check-r1--accept-stage-2).  
**Проект:** [IP-001](../../README.md) · **журнал этапов:** [DECISIONS.md](./DECISIONS.md).

## Что действует сейчас

| Этап | Статус | Действующий результат / решение |
|---|---|---|
| Stage 0 — карта корпуса | принят | [`rr-000_Acts_Stage0_Corpus_Map-R1.md`](./rr-000_Acts_Stage0_Corpus_Map-R1.md); принят в историческом [RUN.md](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md) |
| Stage 1 — первичные наблюдения | принят | [`rr-001_Acts_Primary_Observations.md`](./rr-001_Acts_Primary_Observations.md); [Event 060](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-060--project-lead-acceptance-acts-rr-stage-1-primary-observation) |
| Stage 2 — карта повторений | **принят** | [`rr-002_Acts_Repetition_Stable_Evidence_Map-R1.md`](./rr-002_Acts_Repetition_Stable_Evidence_Map-R1.md); [Event 072](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-072--ip-001-acts-rr-lead-focused-re-check-r1--accept-stage-2) |
| Stage 3 — предварительная классификация | подготовлен; **не активирован** | [пакет задания и договор v0.1](../../Planning/ACTS-Stage-3-Assignment-Package-v0.1.md); [ACTS-D002](./DECISIONS.md#acts-d002--подготовка-задания-stage-3-исполнение-не-разрешено); требуется отдельное разрешение Owner |
| Verification и Stage 4 — книжный итог | не активированы | предметная проверка и независимый аудит книжного закрытия имеют отдельные зависимости |

**Открытые вопросы:** `V01, V03, V04, V05, V10, V11, V12, V13, V14, V18 + O03`. Принятие Stage 2 не разрешило их.  
**Следующий шаг:** Owner утверждает/возвращает/откладывает подготовленный пакет и отдельно решает о контролируемом исполнении Stage 3 рабочей веткой Researcher IP-001; будущая приёмка — у рабочей ветки Lead IP-001. Подготовка не активирует роли; ownership после handoff — Owner.  
**Историческое сравнение:** запрещено до установленного отдельного gate.  
**Книжное закрытие:** не достигнуто.

## Как различать файлы этой папки

| Префикс / имя | Значение и статус |
|---|---|
| `research-000.md`, `doc-*`, `Summary.md`, `Book.md` | прежний исследовательский цикл, перенесённый без изменения содержания; сохраняется для происхождения и возможного будущего сравнения |
| `rr-000_Acts_Stage0_Corpus_Map.md` | прежняя редакция Stage 0; принятой является R1 в таблице выше |
| `rr-002_Acts_Repetition_Stable_Evidence_Map.md` | исходная редакция Event 062; была возвращена для ограниченной языковой коррекции |
| `rr-002_Acts_Repetition_Stable_Evidence_Map-R1.md` | цельная заменяющая редакция, **принятая Event 072** |

`R1` означает номер редакции, а не автоматическое признание результата. При новой коррекции действующий файл меняется только после нового полномочного решения и обновления этого паспорта.

## Основание и границы

Свежий книжный цикл установлен [Installation Package R1](../../../../Development/Validation-Runs/RL-WAVE-2/Artifacts/IP-001-ACTS-Book-Cycle-Installation-Package-R1.md), [Protocol IP-001 v0.2](../../IP-001_Protocol_v0.2.md) и конкретными назначениями в историческом [RL-WAVE-2/RUN.md](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md). Принятые результаты сохраняют свои исходные версии управляющих документов. Для новых назначений действует [Методология v0.4](../../../../Methodology/methodology_v0.4.md) в пределах явно установленной конфигурации.

Исходное поколение `doc-*` и книжные сводки не служат ключом ответов для свежих `rr-*`. Исходная `rr-002` и предыдущая редакция R1 в истории commits остаются доступными как provenance. Принятая R1 не является независимой предметной проверкой всей книги и не запускает Stage 3.

**Ответственный за актуальность этого паспорта:** Project Lead при принятии/возврате этапа; [правило обновления](../../../../Processes/Documentation_and_Decision_Records.md).
