# AI Team Playbook

[Deutsch (Standard)](README.md) | English

A public library of adaptable processes, standards, and templates for
collaboration between people and AI agents.

The playbook makes shared ways of working visible, verifiable, and reusable. It
is not a universal company handbook: each team decides which content to adopt,
adapt, and make binding.

## Process overview

| Process | What does it govern? | When is it useful? | Use case |
| --- | --- | --- | --- |
| [Collaboration between people and AI agents](docs/prozesse/zusammenarbeit-mensch-ki.en.md) | Task ownership, status updates, handoffs, AI reviews, and follow-up work | When several people with their own AI agents work on shared changes | [GitHub with local Claude clients](docs/anwendungsfaelle/teamprozess-mensch-ki-github.en.md) |
| [Lifecycle of shared applications](docs/prozesse/anwendungs-lebenszyklus.en.md) | Idea, classification, trial, operational handover, regular review, and retirement | When an idea may become a shared and maintained application | [App lifecycle in a company](docs/anwendungsfaelle/gedankenspiel-app-lifecycle.en.md) |

The processes are generally applicable and written independently of tools and
organizations; the same applies to the standards below. Use cases show how a
process can be implemented in a specific context. All content has the status Draft: these are proposals whose practical
use has not yet been proven.

## Standards

| Standard | What does it govern? |
| --- | --- |
| [Approval boundaries for AI agents](docs/standards/freigabegrenzen-fuer-agenten.en.md) | What an agent may do on its own and what requires human approval |
| [Evidence instead of self-assessment](docs/standards/nachweis-statt-selbsteinschaetzung.en.md) | Completion reports with observed check results, unknowns marked |
| [Data and confidentiality when using AI](docs/standards/daten-und-vertraulichkeit.en.md) | Which data may go to which AI tools, protection of credentials |
| [Agent configuration as a maintained artifact](docs/standards/agent-konfiguration.en.md) | Agent rules and skills versioned in the project, with review and a way back |
| [Labeling AI contributions](docs/standards/kennzeichnung-von-ki-beitraegen.en.md) | When and how AI contributions become visible in commits, change proposals, and reviews |

## Use the playbook

1. Select a suitable starting point from the process overview.
2. Read the process problem, roles, prerequisites, and limits.
3. Adapt terminology and workflow to the team's context.
4. Decide within the team which parts become binding.
5. Document experience and change needs traceably.

The [vision](vision.en.md) describes the project's purpose, target state, and
principles. Content structure, status model, and maintenance are defined in the
[documentation structure](docs/README.en.md).

## Templates and skills

| Resource | Purpose |
| --- | --- |
| [Content template](docs/vorlagen/inhalt.en.md) | Structure a new process or standard consistently |
| [Change request](docs/vorlagen/aenderungsanfrage.en.md) | Record the problem, goal, scope, and decision traceably |
| [Pull request template](docs/vorlagen/pull-request.en.md) | Summarize a change and its verification evidence for review |
| [Project-local skills](AGENTS.en.md#select-the-appropriate-skill) | Guide AI agents through creating, adapting, and checking content |

## Languages

German is the default language and uses file names without a language suffix.
English versions live beside them and use `.en.md`. Both versions are maintained
together and link to one another.

## Contributing

Before contributing new material, check whether content with the same purpose
already exists. A change proposal should describe the concrete problem, desired
result, and verifiable completion. Public content is always changed in German and
English together.

The [project rules](AGENTS.en.md) contain the complete maintenance and
verification requirements.

## License

Documentation, processes, templates, and skills are licensed under
[CC BY 4.0](LICENSES/CC-BY-4.0.txt). Software and executable scripts are licensed
under [Apache-2.0](LICENSES/Apache-2.0.txt). See the
[licensing overview](LICENSE.en.md) for the exact allocation and attribution guidance.
