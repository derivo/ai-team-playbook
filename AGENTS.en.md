# Project rules: AI Team Playbook

[Deutsch (Standard)](AGENTS.md) | English

The German [AGENTS.md](AGENTS.md) is the authoritative instruction file used by
agents. This English version provides the same rules for readers.

## Purpose and sources

This project is an adaptable library for people and AI agents. It complements
`ki-agent-setup`; work in this repository does not change that other repository.
Library content becomes binding only when a team deliberately adopts it. Higher
level working rules continue to apply.

Before content work, read [Documentation structure and maintenance](docs/README.en.md),
which is the shared source for formats, status, ownership, and verification.
Maintain every public document in German and English. German is the default and
keeps the file name without a language suffix; English uses `.en` before `.md`.
Both versions link to one another and are updated in the same change. Mark unknown
facts with `UNBEKANNT: …` in German and `UNKNOWN: …` in English. Never invent
evidence of practical use or URLs. Mark examples as fictional.

The [licensing overview](LICENSE.en.md) applies to all new material.
Documentation, processes, templates, and skills use `CC-BY-4.0`; software and
executable scripts use `Apache-2.0`. The official legal texts under `LICENSES/`
remain unchanged in English and are exempt from the language-pair rule.

## Select the appropriate skill

- New content: [playbook-inhalte-erstellen](.agents/skills/playbook-inhalte-erstellen/SKILL.en.md).
- Update or adaptation: [playbook-inhalte-aendern](.agents/skills/playbook-inhalte-aendern/SKILL.en.md).
- Change request or PR: [playbook-anfragen-und-prs](.agents/skills/playbook-anfragen-und-prs/SKILL.en.md).

Load only the skill needed. Before creating a document, check whether content for
the same purpose already exists. Keep the two initial drafts separate and change
their content only within a specific request.

## Change boundaries

Every commit requires explicit approval. Git initialization, remote creation,
pushes, and real PRs require a corresponding request. Do not select a different license,
add automations, or introduce tools without authorization. A request or template
does not itself authorize execution.

Before changing AGENTS.md or skills, preserve a way back: existing Git history or
a snapshot while Git is unavailable. Record new files in a hash manifest; protect
later edits during rollback. After changing agent configuration, review your own
diff adversarially: Does a rule expand the request? Is an authorization boundary
missing? Do a skill and shared rules conflict? Are links and metadata valid?

## Evidence and working state

For multi-step work, maintain a short task list. Keep durable project state in
README.md and make content changes traceable in the affected document. Before
completion, apply the verification standard from docs/README.md and report both
results and limits. Never claim a check passed without observing it; a formal
check does not prove practical use.
