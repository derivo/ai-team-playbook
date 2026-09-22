# AI Team Playbook

[Deutsch (Standard)](README.md) | English

**Status: Draft**

A library of adaptable standards, processes, and workflows for collaboration
between people and AI agents. It complements `ki-agent-setup` with team
workflows. Each team decides for itself how to adapt the material and whether to
make it binding.

[Vision and continuation guide](vision.en.md) describe the target state, the
verified working state, and the next steps toward an initial publication.

## Initial drafts

- [Team process: Issues, pull requests, and AI reviews](docs/entwuerfe/teamprozess-mensch-ki-github.en.md)
- [Thought experiment: From app idea to retirement](docs/entwuerfe/gedankenspiel-app-lifecycle.en.md)

The documents are independent proposals and are not presented as proven practice.

## Editing content

[Documentation structure and maintenance](docs/README.en.md) define formats,
status values, and verification criteria. [Project rules](AGENTS.en.md) explain
the working rules; German remains their authoritative default.

Project-local skills:

- [playbook-inhalte-erstellen](.agents/skills/playbook-inhalte-erstellen/SKILL.en.md): create new content.
- [playbook-inhalte-aendern](.agents/skills/playbook-inhalte-aendern/SKILL.en.md): update content or adapt it to a specific context.
- [playbook-anfragen-und-prs](.agents/skills/playbook-anfragen-und-prs/SKILL.en.md): prepare change requests and pull requests.

Supporting clients can invoke the skills by name or use them as working
instructions. They do not install automations.

## Working state

The bilingual foundation has been prepared. Git uses `main`; the public
repository is [derivo/ai-team-playbook](https://github.com/derivo/ai-team-playbook).
German is the default language, while English files use the `.en.md` suffix. No
license has been selected. Library maintainer: UNKNOWN. Next review: before the
first practical trial.
