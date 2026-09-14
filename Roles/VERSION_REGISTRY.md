# Research Lab — Role Version Registry

**Registry version:** 0.1  
**Status:** Current  
**Updated:** 14.09.2026  
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
| Research Lab Director | v0.1 | Candidate Active | yes | pending |
| Research Project Lead | v0.1 | Candidate Active | yes | pending |
| Researcher | v0.1 | Candidate Active | yes | pending |
| Research Auditor | v0.1 | Candidate Active | yes | pending |

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

Until evidence changes this registry, every v0.1 role remains validation-pending.
