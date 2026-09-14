# Research Lab — Role Package Versioning and Evolution Standard v0.1

**Status:** Research Lab Pilot Standard  
**Validation:** pending

## Principle

Several versions of one role may remain active because different Research Projects can be long-running.

The canonical authority is the Version Registry, not an unversioned mutable role file.

## Role Configuration Lock

Each active Stage or Assignment pins role core version, Package A/B/C, mode versions or embedded mode definitions, Protocol version, Output Contract, project overlay and installation date.

## Adoption outcomes

- CONTINUE PINNED
- ADOPT COMPATIBLE PATCH
- MIGRATE AT STAGE BOUNDARY
- MANDATORY MIGRATION

No new version silently changes active work.

## Change classes

- **Local Capability Delta** — bounded lesson that does not change shared identity.
- **Project Overlay** — project-specific requirement recorded in Protocol or Assignment.
- **Compatible Patch** — non-breaking clarification adopted explicitly.
- **Role Revision** — material change to identity, authority, boundaries, recovery or required outputs; creates a new version.

## During active work

A role may report a Capability Gap at any time. The process may continue pinned when safe. Director determines whether the gap belongs to Assignment correction, Project Overlay, compatible patch, new role version, Methodology proposal or Constitution proposal.

## Archive

A version moves to Archived only when no active Research Project or Stage uses it. Prefer logical status and stable versioned paths so provenance and links remain reproducible.

## Promotion boundary

This standard is tested first inside Research Lab. It does not automatically migrate Publication System or become a project-wide In Profundo standard.
