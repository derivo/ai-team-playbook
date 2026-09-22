# Vision: AI Team Playbook

[Deutsch (Standard)](vision.md) | English

- Status: Draft
- Maintainer: maintainer team (reviews changes)
- Content checked: 2026-09-22 against the local project state
- Next review trigger: before the start version or when the project goal changes
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

Processes and standards are generally applicable and written independently of
tools, agents, and organizations. Real use cases are derived from them, such as
working with GitHub in a company where colleagues use their own Claude clients.
A use case links to its process and describes only what is specifically
different or more precise in its context.

Project-local skills guide people and agents through creating, adapting, and
changing content. Change requests and pull requests connect the need, decision,
implementation, and verification evidence. Experience is described as such only
when its context and outcome have been documented.

The library complements `ki-agent-setup` while remaining an independent project.
Teams adopt only the parts they deliberately select and adapt.

## Roles

- The maintainer team keeps structure, status, and references current and
  reviews changes. In a fork or copy, the adopting team names its own
  maintainers.
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
- Two general processes are stored under `docs/prozesse/`. The two adopted
  initial drafts are stored as use cases under `docs/anwendungsfaelle/` and link
  to their process.
- Content, change request, and pull request templates are stored under
  `docs/vorlagen/`.
- Three project-local skills support creation, adaptation, requests, and pull
  requests.
- Git is initialized with the `main` branch. The public remote
  [derivo/ai-team-playbook](https://github.com/derivo/ai-team-playbook) is
  configured as `origin`. The bilingual foundation is the first publication;
  no pull requests exist yet.
- Licensing is defined: editorial material uses `CC-BY-4.0`, while software and
  executable scripts use `Apache-2.0`. The maintainer team maintains the library.

This section is a snapshot. On continuation, verify every statement against the
actual project state.

## Process toward the start version

### 1. Review content and boundaries

Status: reviewed and implemented on 2026-09-22; two points remain open.

Review both initial drafts, the templates, the skills, and this vision together.
Record open changes. Acceptance criterion: project
purpose, audience, boundaries, and initial content do not contradict one another;
remaining disagreements are documented explicitly.

Result: the drafts were tied to one company and specific tools. The decision was
to write processes as generally applicable and to keep the drafts as use cases.
Until the start version, changes are made directly in the repository; afterwards
they are recorded as GitHub issues. Open:

- UNKNOWN: criterion for when the start version counts as finished.
- UNKNOWN: who takes the content owner role. Decided: new content is maintained
  by the maintainer team by default.

### 2. Decide maintenance and license

Status: completed on 2026-09-22.

The maintainer team maintains the library. Licensing was defined on 2026-09-22
as `CC-BY-4.0` for editorial material and `Apache-2.0` for software. Acceptance
criterion: ownership is documented and new files follow the defined license
allocation.

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
4. Name the first unfinished step under “Process toward the start version” and
   work only on its prerequisites.
5. Do not select another license, create a commit, push, or publish unless that
   action has been explicitly requested or approved.
6. After the work, update vision.md and vision.en.md only where verified state,
   a decision, or the next step actually changed.
```

## Templates

- [Content template](docs/vorlagen/inhalt.en.md)
- [Change request template](docs/vorlagen/aenderungsanfrage.en.md)
- [Pull request template](docs/vorlagen/pull-request.en.md)

## Limits

This vision is neither a binding schedule nor authorization to publish. It does
not select a technical platform beyond the documented GitHub workflow; licensing
is governed by the [license overview](LICENSE.en.md). It makes no claim of practical use and does not replace a specific
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
- 2026-09-22: Recorded licensing (`CC-BY-4.0` for editorial material,
  `Apache-2.0` for software), assigned the maintainer team as maintainer, and
  marked step 2 as completed.
- 2026-09-22: Completed step 1: created general processes under
  `docs/prozesse/`, moved the initial drafts to `docs/anwendungsfaelle/` as use
  cases, and aligned the process with the start version.
- 2026-09-22: Set the maintainer team as default maintainer for new content in
  the template, documentation structure, and skill.
