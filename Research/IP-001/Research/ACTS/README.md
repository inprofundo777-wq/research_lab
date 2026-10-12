# IP-001 — Деяния апостолов

**Состояние:** свежий проход Stage 0–3 принят; snapshot закреплён; пакет Material Verification подготовлен, исполнение не разрешено; ownership — Owner.  
**Сверено:** 12.10.2026 по [ACTS-D006](./DECISIONS.md#acts-d006--lead-ограниченный-пакет-material-verification-представлен-owner); Stage 3 принят ACTS-D005; разрешение — ACTS-D003; приёмка Stage 2 — [Event 072](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-072--ip-001-acts-rr-lead-focused-re-check-r1--accept-stage-2).  
**Проект:** [IP-001](../../README.md) · **журнал этапов:** [DECISIONS.md](./DECISIONS.md).

## Что действует сейчас

| Этап | Статус | Действующий результат / решение |
|---|---|---|
| Stage 0 — карта корпуса | принят | [`rr-000_Acts_Stage0_Corpus_Map-R1.md`](./rr-000_Acts_Stage0_Corpus_Map-R1.md); принят в историческом [RUN.md](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md) |
| Stage 1 — первичные наблюдения | принят | [`rr-001_Acts_Primary_Observations.md`](./rr-001_Acts_Primary_Observations.md); [Event 060](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-060--project-lead-acceptance-acts-rr-stage-1-primary-observation) |
| Stage 2 — карта повторений | **принят** | [`rr-002_Acts_Repetition_Stable_Evidence_Map-R1.md`](./rr-002_Acts_Repetition_Stable_Evidence_Map-R1.md); [Event 072](../../../../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-072--ip-001-acts-rr-lead-focused-re-check-r1--accept-stage-2) |
| Stage 3 — предварительная классификация | **COMPLETE / ACCEPTED — предварительные группы** | [rr-003 — закреплённый target](https://github.com/inprofundo777-wq/research_lab/blob/18b300ae11beeeccc483d75196fd3c9ca7914287/Research/IP-001/Research/ACTS/rr-003_Acts_Provisional_Groups.md); [ACTS-D005 — приёмка](./DECISIONS.md#acts-d005--lead-accept-stage-3-и-фиксация-fresh-snapshot); разрешение ACTS-D003 |
| Material Verification | пакет подготовлен; **исполнение не разрешено** | [ACTS-MV-PACK-v0.1](../../Planning/ACTS-Material-Verification-Package-v0.1.md); ACTS-D006; сначала отдельный gate capability, затем MV |
| Stage 4 / книжное закрытие | не активированы | предметная проверка и независимый аудит книжного закрытия имеют отдельные зависимости |

**Открытые вопросы:** `V01, V03, V04, V05, V10, V11, V12, V13, V14, V18 + O03`. Принятие Stage 2–3 не разрешило их.  
**Следующий шаг:** Owner рассматривает подготовленный MV-пакет; рекомендован Gate A — подтвердить конкретную независимую конфигурацию и разрешить только capability probe U04/U12/D20. Производственная MV требует отдельного Gate B после оценки допуска. **Ownership — Owner.** [Fresh Stage 0–3 snapshot](../../Planning/ACTS-Fresh-Stage-0-3-Snapshot-2026-10-12.md) закреплён; он и приёмка Stage 3 не разрешают следующий этап.  
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
