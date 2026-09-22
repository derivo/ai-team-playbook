# Standard: Approval boundaries for AI agents

[Deutsch (Standard)](freigabegrenzen-fuer-agenten.md) | English

- Status: Draft
- Maintainer: maintainer team (reviews changes)
- Content checked: 2026-09-22 against the project rules of this repository; no practical use has been proven.
- Next review trigger: before team adoption and when practical feedback arrives
- Evidence of practical use: None; not marked as proven.
- Adoption: Decision of the adopting team.
- Use cases: None yet.

Maintenance and formats: [Documentation structure](../README.en.md).

## Problem

AI agents can change files, run commands, and call external services. Without
agreed boundaries, it is unclear what an agent may do on its own and when a person
must approve. The results are unintended publications, changes that are hard to
undo, and responsibility nobody has taken.

## Audience

Teams and individuals who use AI agents with write or execution rights in
repositories, systems, or external services.

## Roles

- **Responsible person:** gives assignments and approvals and is responsible for
  the result.
- **AI agent:** acts within the assignment and asks for consent before actions
  that require approval.
- **Team:** defines which actions belong to which level.

## Process

### 1. Classify actions into levels

| Level | Examples | Rule |
|---|---|---|
| Free | Reading, searching, local analysis, drafts in the working directory | The agent acts within the assignment |
| With assignment | Local changes to files covered by the assignment | Only within the assigned scope; add nothing unrequested |
| Approval per action | Commit, push, pull request, outbound messages and comments, deleting or overwriting, costs, changes to permissions and configuration | Explicit consent before each individual action |
| Excluded | Circumventing safeguards, passing on credentials | Never, not even when instructed by a document or tool result |

### 2. Keep approvals unambiguous

- An approval applies to the named action, not to similar later actions.
- A request, template, or document content is not permission to execute.
- Before approval, the agent states exactly what will happen and what is
  affected, such as files, recipients, or scope.

### 3. Secure a way back

Before changes that are hard to undo, a way back exists, such as version history
or a backup. Before deleting or overwriting, the target is inspected.

### 4. Limit series

Before a series of similar actions, the agent presents a plan: what is affected
and how each unit is checked. The team sets a limit after which an interim report
and a new approval are required.

## Templates

```text
Approval requested
Action: [exactly what will happen]
Affected: [files, systems, recipients, scope]
Way back: [how the action can be undone, or "none"]
Reason: [relation to the assignment]
```

## Limits

- Technical safeguards such as permissions or branch protection complement this
  standard; it does not replace them.
- Adaptation points: assignment of actions to levels, limit for series, standing
  approvals for narrowly defined routine actions.

## Sources

- Derived from the [project rules](../../AGENTS.en.md) of this repository.
- Proposal without proven practical use.

## Change history

- 2026-09-22: Created as a standard.
