# Documentation structure and maintenance

[Deutsch (Standard)](README.md) | English

## Purpose and audience

This library provides teams and AI agents with adaptable standards, processes,
and workflows. Readers should be able to find a suitable draft, understand its
limits, and document a deliberate adaptation for their context.

## Scope and sources

The library contains documents, templates, and skills for maintaining content.
It does not contain installed automations or a binding company handbook. Sources
are the specific change request, the affected documents, and evidence that was
actually verified. Experience is never invented.

## Locations and formats

- [Project overview](../README.en.md): purpose, entry point, status, and working state.
- [Vision and continuation guide](../vision.en.md): target state, current state, and next steps.
- [Project rules](../AGENTS.en.md): rules for work in this repository; German is authoritative.
- `prozesse/`: generally applicable processes and standards, independent of tools and organizations.
- `anwendungsfaelle/`: specific implementations of a process in a named context.
- `erprobungen/`: plan, observations, and result of a practical trial.
- [Content template](vorlagen/inhalt.en.md): structure for new or adapted content.
- [Change request](vorlagen/aenderungsanfrage.en.md): usable locally and later as an issue.
- [Pull request template](vorlagen/pull-request.en.md): local PR draft and later a pull request.
- `.agents/skills/`: project-local skills for content, revisions, requests, and PRs.

Documents use UTF-8 Markdown (`.md`), one H1 heading, and logically ordered H2/H3
sections. File names are descriptive, lowercase, and hyphenated. Links are
relative; external URLs are included only after verification. Code fences name
their language; form text uses `text`. Tables are reserved for actual
comparisons. Do not introduce a tool dependency solely for documentation upkeep.

Every public document is a language pair. The German default keeps the file name
without a language suffix, such as `vision.md`. The English version uses
`.en.md`, such as `vision.en.md`. Both files live in the same directory, link to
one another near the top, and represent the same substantive state. A content
change is complete only after both versions have been updated and checked.

The official legal texts under `LICENSES/` are unchanged English originals and
the sole exception to the language-pair rule. The allocation of `CC-BY-4.0` and
`Apache-2.0` is defined in the [licensing overview](../LICENSE.en.md).

New content follows: **Problem → Audience → Roles → Process → Templates →
Limits**. Maintenance metadata precedes these sections; sources and change
history follow them. General processes and standards describe roles and
procedures without tying them to a specific tool, agent, or organization. A use
case describes a specific implementation in a named context, links to its general
process in its header, and may use its own structure. Context-specific content
belongs in the use case, not in the process. The two adopted use cases retain
their source text; restructuring them requires a specific request.

## Status and adoption

| Status | Requirement |
| --- | --- |
| Draft | Proposal; no claim of proven practice |
| proven | Context, date, approach, result, and limits of the trial are documented |
| superseded | Date, reason, and successor link, or an explicit statement that none exists |

These values describe document maturity, not issue progress or an app's operating
state. When a proven document changes, check whether its evidence still applies;
otherwise reset it to Draft. Superseded content retains the earlier decision.

Each team decides which parts to adopt and make binding. “Must” inside a process
draft applies to that proposed process; inclusion in this library does not bind a
team by itself.

## Ownership and review

Each document names its status, maintainer, last substantive review, next review
trigger, and evidence of practical use. Unless specified otherwise, the
maintainer team maintains the document; enter different ownership only on
request and never invent a person. Maintainers review a document when
sources change, practical feedback arrives, or a team prepares to adopt it. The
adopting team names responsible people and an appropriate next review date. An
agent may support the review but cannot replace a human decision.

## Changes and requests

Before changing content, check existing documents and open requests. When a
request is created locally, copy the request template under a unique descriptive file name and use relative
links. A request records the problem, goal, scope, acceptance criteria, and
decision. Implemented changes receive a short change-history entry; details live
in the linked request rather than in parallel records.

Until a finished start version exists, changes are made directly in the
repository. After that, requests become GitHub issues and changes become linked
pull requests. Reuse local requests and link to the migrated issue. Never invent issue
numbers, pull requests, or URLs. A pull request draft does not authorize a commit,
push, or publication. Record concrete follow-up work as separate, mutually linked
requests; preserve rejected requests with a reason. When using the team process,
its more specific follow-up issue rules apply.

## Verification standard

Before completion, check Markdown and skill metadata mechanically, resolve
relative links, compare claims with their sources, and scan changes for secrets
or real personal data. Examples are explicitly fictional. Diagrams require a
render check if any are added. Run existing formatters only on changed files.
Name missing tools and the limits of substitute checks; never claim that
everything was checked without evidence.

A change is complete when its observed checks pass, its acceptance criteria are
met, and open points are named. A document can remain a Draft after successful
documentation checks because those checks do not prove practical use.
