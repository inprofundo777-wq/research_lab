# Research Lab — Role Version Registry

**Registry version:** 0.1  
**Status:** Current  
**Updated:** 24.09.2026  
**Authority:** canonical registry for active Research Lab role package versions

## Status vocabulary

- **Candidate** — drafted but not active.
- **Candidate Active** — may be used only in controlled validation.
- **Active** — validated for defined use.
- **Default** — preferred active version for new compatible work.
- **Supported** — valid for pinned existing work.
- **Deprecated** — no new adoption; existing work may continue if explicitly allowed.
- **Retired** — must not be activated.
- **Archived** — no active process uses the version.

## Current versions

| Role | Version | Status | Default for new validation | Validation |
|---|---:|---|---|---|
| Research Lab Director | v0.1 | Scoped Active | yes, within scope | broader modes pending |
| Research Project Lead | v0.1 | Scoped Active | yes, within scope | broader modes pending |
| Researcher | v0.1 | Scoped Active | yes, within scope | broader modes pending |
| Research Auditor | v0.1 | Scoped Active | yes, within scope | broader modes pending |

## Scoped Active envelope

Owner approved the following exact production-use envelope in `RL-WAVE-2`, Event 037:

| Role | Scoped Active use | Validation Pending |
|---|---|---|
| Research Lab Director v0.1 | bounded Formation; route and close recommendations under an explicit Owner gate | all other modes and uses |
| Research Project Lead v0.1 | bounded Installation; Stage Coordination; Output Contract acceptance | all other modes and uses |
| Researcher v0.1 | Existing Research Coverage Review; limited scholarly synthesis; bounded textual probe | all other research modes and methods |
| Research Auditor v0.1 | Formation Audit; Installation Audit | all other audit modes, including independent audit of late-stage research conclusions |

`Scoped Active` is not unrestricted production authority. Every activation must still pin Package, modes, Protocol, Output Contract, authority envelope and return route.

**Decision source:** [RL-WAVE-2 — Event 037](../Development/Validation-Runs/RL-WAVE-2/RUN.md#event-037--owner-decision-on-scoped-active-transition)

## Active paths

- Director/v0.1/
- Project-Lead/v0.1/
- Researcher/v0.1/
- Auditor/v0.1/

## Rule

A Project, Stage, Assignment or Output must pin the exact role version, Package A/B/C, activated modes, Protocol version and Output Contract version.

A new version does not silently change an active process.

## Validation route

~~~text
Fresh-context Recovery
→ Formation Pilot
→ Installation Pilot
→ Micro Research Cycle
→ Review / Re-check
→ Book Cycle Pilot
→ Knowledge Transfer Pilot
→ System Review
~~~

Only the exact envelope above is Active. Everything outside it remains Validation Pending until new evidence and an explicit Owner decision change this registry.
