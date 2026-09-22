# Vision: AI Team Playbook

[Deutsch (Standard)](vision.md) | English

- Status: Draft
- Maintainer: UNKNOWN: not assigned
- Content checked: 2026-09-22 against the local project state
- Next review trigger: before the first publication or when the project goal changes
- Evidence of practical use: None; the library has not been tested in practice.
- Adoption: Each adopting team decides for itself.

## Problem

Teams often develop their own rules for collaboration between people and AI
agents in isolated chats, local files, or separate projects. Decisions, templates,
and lessons are then lost or recreated. After an interruption, it is often
unclear what has already been prepared, which decisions remain open, and which
step should happen next.

The AI Team Playbook aims to provide a public, traceably maintained library for
this work. It collects adaptable standards, processes, and workflows without
automatically turning them into binding company policy.

## Audience

The library is for teams that have people and AI agents work together on
software, documentation, or operational processes. It should allow both people
and agents to:

- find a suitable process quickly,
- understand its maturity and limits,
- adapt it deliberately to their context, and
- pass changes on with verifiable reasons and evidence.

## Target state

The repository contains a small, understandable collection of independent
playbook documents. Each document describes the problem, audience, roles,
process, directly usable templates, and limits. Its status shows whether it is a
draft, has been proven in a documented context, or has been superseded.

Project-local skills guide people and agents through creating, adapting, and
changing content. Change requests and pull requests connect the need, decision,
implementation, and verification evidence. Experience is described as such only
when its context and outcome have been documented.

The library complements `ki-agent-setup` while remaining an independent project.
Teams adopt only the parts they deliberately select and adapt.

## Roles

- The library maintainer keeps structure, status, and references current. This
  role has not been assigned.
- Content owners review individual processes and their evidence when changes or
  practical feedback occur.
- Contributors describe change needs traceably and supply suitable evidence.
- Adopting teams decide how to adapt material and whether to make it binding.
- AI agents support research, creation, and verification but do not make
  organizational decisions in place of a person.

## Current state

The following local state was checked on 2026-09-22:

- The project directory `/Users/dennis/code/ai-team-playbook` exists.
- [Project overview](README.en.md), [project rules](AGENTS.md), and
  [documentation structure](docs/README.en.md) exist.
- Two separate initial drafts are stored under `docs/entwuerfe/`.
- Content, change request, and pull request templates are stored under
  `docs/vorlagen/`.
- Three project-local skills support creation, adaptation, requests, and pull
  requests.
- Git is initialized with the `main` branch. The public remote
  [derivo/ai-team-playbook](https://github.com/derivo/ai-team-playbook) is
  configured as `origin`. The bilingual foundation is the first publication;
  no pull requests exist yet.
- No license or library maintainer has been selected.

This section is a snapshot. On continuation, verify every statement against the
actual project state.

## Process toward the first publication

### 1. Review content and boundaries

Review both initial drafts, the templates, the skills, and this vision together.
Record open changes as local change requests. Acceptance criterion: project
purpose, audience, boundaries, and initial content do not contradict one another;
remaining disagreements are documented explicitly.

### 2. Decide maintenance and license

Name a human maintainer and deliberately select a license. An agent must not make
the license decision in advance. Acceptance criterion: ownership and the license
decision are documented; the license file is created only after that decision.

### 3. Prepare version control

Status: completed on 2026-09-22 for the first publication.

After an explicit request, initialize Git, inspect the local state, and obtain
separate approval before a commit. Acceptance criterion: the proposed commit
contains only reviewed project files and no secrets or temporary working files.

### 4. Prepare publication

Status: completed on 2026-09-22 with the public repository
`derivo/ai-team-playbook`.

After an explicit request, configure a public remote. Before pushing, verify the
repository name, visibility, default branch, README, license, and links.
Acceptance criterion: the remote matches the decisions and the local branch has
an unambiguous upstream. Push and publication cover only the explicitly approved
scope.

### 5. Trial one document

A team selects a draft, adapts it to a named context, and documents the period,
approach, result, and limits. Acceptance criterion: an uninvolved person can
understand what was tried and which claims the evidence supports. Only then may
the document receive the status `proven`.

### 6. Establish a maintenance cycle

Record feedback as change requests, review changes through pull requests, and
retain superseded content with its reason and successor. Acceptance criterion:
every active document shows a maintainer and next review trigger.

## Continuation template

Start a new session with this block:

```text
Goal: Continue work on the AI Team Playbook at the first unfinished step.
Project: /Users/dennis/code/ai-team-playbook

1. Read AGENTS.md, vision.md, vision.en.md, README.md, and docs/README.md in full.
2. Inspect project files and, if present, git status; do not trust this snapshot
   without verification.
3. Find existing change requests and open decisions.
4. Name the first unfinished step under “Process toward the first publication”
   and work only on its prerequisites.
5. Do not select a license, initialize Git, create a commit, configure a remote,
   or publish unless that action has been explicitly requested or approved.
6. After the work, update vision.md and vision.en.md only where verified state,
   a decision, or the next step actually changed.
```

## Templates

- [Content template](docs/vorlagen/inhalt.en.md)
- [Change request template](docs/vorlagen/aenderungsanfrage.en.md)
- [Pull request template](docs/vorlagen/pull-request.en.md)

## Limits

This vision is neither a binding schedule nor authorization to publish. It does
not select a license or a technical platform beyond the documented GitHub
workflow. It makes no claim of practical use and does not replace a specific
change request.

The library should remain small and adaptable. New content starts from a concrete
need; automations, integrations, and additional variants are not created in
advance.

## Sources

- The local project state observed on 2026-09-22
- [Project overview](README.en.md)
- [Project rules](AGENTS.en.md)
- [Documentation structure and maintenance](docs/README.en.md)
- The request to enable seamless continuation later

## Change history

- 2026-09-22: Initial draft created with target state, verified starting state,
  publication path, and continuation template.
