# Standard: Agent configuration as a maintained artifact

[Deutsch (Standard)](agent-konfiguration.md) | English

- Status: Draft
- Maintainer: maintainer team (reviews changes)
- Content checked: 2026-09-22 against the project rules of this repository; no practical use has been proven.
- Next review trigger: before team adoption and when practical feedback arrives
- Evidence of practical use: None; not marked as proven.
- Adoption: Decision of the adopting team.
- Use cases: None yet.

Maintenance and formats: [Documentation structure](../README.en.md).

## Problem

How an AI agent behaves in a project depends on its instructions: rule files,
skills, settings. If they exist only locally with individuals, agents in the same
project follow different rules. Unreviewed changes can weaken approval boundaries
without anyone noticing.

## Audience

Teams in which several people use AI agents in the same project.

## Roles

- **Maintainers:** keep the project configuration current and review changes to
  it.
- **Contributors:** propose configuration changes like any other content.
- **AI agent:** reads the project configuration and changes it only on request.

## Process

### 1. Store configuration in the project

Project rules for agents are versioned in the repository, for example in an
`AGENTS.md`. Tool-specific files refer to this shared source instead of copying
rules. Project-specific skills are also stored in the repository.

### 2. Separate shared and personal rules

Personal settings stay local. What applies to everyone in the project belongs in
the project configuration. In case of conflict, the project rule takes precedence
unless the team decides otherwise.

### 3. Review changes

Changes to rules, skills, or settings go through the same review as other
changes. The review specifically checks:

- Does a rule expand the assignment or the powers of an agent?
- Is an approval boundary missing or weakened?
- Do rules, skills, and shared requirements contradict each other?
- Are references and metadata valid?

### 4. Secure a way back

Before a change, a way back exists, usually version history. A configuration
change is kept traceable on its own and not mixed with unrelated content changes.

## Templates

```text
Minimal reference in a tool-specific file:
@AGENTS.md
```

The reference syntax depends on the tool.

## Limits

- The standard does not define the content of the rules, only how they are
  handled.
- Not every tool supports references between files; a maintained copy that names
  its source is then the compromise.
- Adaptation points: file names, location of skills, depth of the review.

## Sources

- Derived from the [project rules](../../AGENTS.en.md) of this repository, whose
  `CLAUDE.md` refers to `AGENTS.md`.
- Proposal without proven practical use.

## Change history

- 2026-09-22: Created as a standard.
