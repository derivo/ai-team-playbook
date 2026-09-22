# AI Team Playbook

Deutsch (Standard) | [English](README.en.md)

**Status: Entwurf**

Eine Bibliothek anpassbarer Standards, Prozesse und Workflows für die
Zusammenarbeit von Menschen und KI-Agenten. Sie ergänzt `ki-agent-setup` um
Teamabläufe. Jedes Team entscheidet selbst über Anpassung und Verbindlichkeit.

[Vision und Wiederaufnahme](vision.md) beschreiben das Zielbild, den belegten
Arbeitsstand und die nächsten Schritte bis zu einer ersten Veröffentlichung.

## Erste Entwürfe

- [Teamprozess: Issues, Pull Requests und KI-Reviews](docs/entwuerfe/teamprozess-mensch-ki-github.md)
- [Gedankenspiel: Von der App-Idee bis zur Abschaltung](docs/entwuerfe/gedankenspiel-app-lifecycle.md)

Die Dokumente sind eigenständige Vorschläge und nicht als Praxiserfahrung belegt.

## Inhalte bearbeiten

[Dokumentstruktur und Pflege](docs/README.md) definieren Formate, Status und
Prüfkriterien. [AGENTS.md](AGENTS.md) legt die Projektregeln fest.

Projektlokale Skills:

- [playbook-inhalte-erstellen](.agents/skills/playbook-inhalte-erstellen/SKILL.md): neue Inhalte verfassen.
- [playbook-inhalte-aendern](.agents/skills/playbook-inhalte-aendern/SKILL.md): Inhalte aktualisieren oder für einen Kontext anpassen.
- [playbook-anfragen-und-prs](.agents/skills/playbook-anfragen-und-prs/SKILL.md): Änderungsanfragen und Pull Requests vorbereiten.

Die Skills können in einem unterstützenden Client über ihren Namen aufgerufen
oder als Arbeitsanleitung gelesen werden. Sie installieren keine Automationen.

## Arbeitsstand

Die zweisprachige Grundlage ist vorbereitet. Git verwendet `main`; das öffentliche
Repository ist [derivo/ai-team-playbook](https://github.com/derivo/ai-team-playbook).
Deutsch ist die Standardsprache, englische Fassungen tragen das Suffix `.en.md`.
Eine Lizenz ist noch nicht festgelegt. Pflegeverantwortung der Bibliothek:
UNBEKANNT. Nächste Prüfung: vor der ersten praktischen Erprobung.
