# Research Lab Role System

**Version:** v0.1 Candidate  
**Status:** 🟡 Implemented / Validation Pending  
**Owner of capability:** Research Lab Director under Owner  
**Authority:** operational execution layer; subordinate to Research Lab Constitution, Methodology and active Project Protocols

## Purpose

Role System defines who performs Research Lab work, within which authority, with which context package, modes, output contract and return route.

It does not define research conclusions and does not create a parallel epistemic authority.

~~~text
DNA
→ Research Lab Constitution
→ Research Lab Methodology
→ Project Protocol
→ Stage Output Contract
→ Research Output

Role System
→ assigns accountable execution inside this hierarchy
~~~

## Core Roles

~~~text
Owner
→ Research Lab Director
→ Research Project Lead
→ Researcher
~~~

Research Auditor remains independent from operational ownership.

## Core distinctions

- **Role** — identity, authority and accountability.
- **Mode** — temporary perspective or capability.
- **Package A/B/C** — depth of installed context.
- **Process Function** — position in a specific lifecycle.
- **Output Contract** — required shape and boundary of a result.

Mode and Package never increase authority.

## Recovery

1. Read this file.
2. Open [Version Registry](./VERSION_REGISTRY.md).
3. Open the selected role version through its README.
4. Read the required Package and activated modes.
5. Read the active Protocol, Assignment and Output Contract.
6. Verify authority, independence and return route.
7. Declare the installed configuration.

Stop if role version, scope, authority, required source, output contract or return route is missing.

## Role indicator

~~~text
▶ Основная роль — [Role]
▶ Основное задание — [Current Assignment]
■ Второстепенная роль — [Role or not activated]
◆ Активные моды — [Modes or none]
~~~

When known parallel branches materially affect the work, add:

~~~text
↔ Известные действующие ветки основной роли — N · [sync state]
~~~

## Standards

- [Installation Standard](./Standards/Installation_Standard_v0.1.md)
- [Authority and Escalation](./Standards/Authority_and_Escalation_v0.1.md)
- [Independence and Audit](./Standards/Independence_and_Audit_v0.1.md)
- [Versioning and Evolution](./Standards/Versioning_and_Evolution_v0.1.md)

## Role entries

- [Research Lab Director](./Director/v0.1/README.md)
- [Research Project Lead](./Project-Lead/v0.1/README.md)
- [Researcher](./Researcher/v0.1/README.md)
- [Research Auditor](./Auditor/v0.1/README.md)

## Current limitation

All v0.1 packages are Candidate Active. Documentation existence is not validation. Initial use is limited to staged recovery, formation, installation, audit and bounded research pilots authorized by Owner.
