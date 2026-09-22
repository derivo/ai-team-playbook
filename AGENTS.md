# Projektregeln: AI Team Playbook

Deutsch (Standard) | [English](AGENTS.en.md)

## Auftrag und Quellen

Dieses Projekt ist eine anpassbare Bibliothek für Menschen und KI-Agenten.
Es ergänzt `ki-agent-setup`; dieses andere Repository wird hier nicht verändert.
Die Bibliotheksinhalte werden erst durch eine Teamentscheidung dort verbindlich.
Übergeordnete Arbeitsregeln bleiben gültig.

Vor Inhaltsarbeit [Dokumentstruktur und Pflege](docs/README.md) lesen; dort liegen
Formate, Status, Zuständigkeit und Prüfmaßstab als gemeinsame Quelle.
Jeden öffentlichen Inhalt auf Deutsch und Englisch pflegen. Die deutsche Fassung
ist der Standard und behält den Dateinamen ohne Sprachsuffix; die englische
Fassung erhält vor `.md` das Suffix `.en`. Beide Fassungen verlinken einander und
werden in derselben Änderung aktualisiert. Unbekanntes auf Deutsch mit
`UNBEKANNT: …`, auf Englisch mit `UNKNOWN: …` markieren. Erfahrungsbelege und
URLs niemals erfinden. Beispiele als fiktiv kennzeichnen.

Die [Lizenzübersicht](LICENSE.md) gilt für alle neuen Inhalte. Dokumentation,
Prozesse, Vorlagen und Skills verwenden `CC-BY-4.0`; Software und ausführbare
Skripte verwenden `Apache-2.0`. Die offiziellen Rechtstexte unter `LICENSES/`
bleiben unverändert auf Englisch und sind von der Sprachpaar-Regel ausgenommen.

## Passenden Skill wählen

- Neuer Inhalt: [playbook-inhalte-erstellen](.agents/skills/playbook-inhalte-erstellen/SKILL.md).
- Aktualisierung oder Anpassung: [playbook-inhalte-aendern](.agents/skills/playbook-inhalte-aendern/SKILL.md).
- Änderungsanfrage oder PR: [playbook-anfragen-und-prs](.agents/skills/playbook-anfragen-und-prs/SKILL.md).

Nur den benötigten Skill laden. Vor einem neuen Dokument nach vorhandenem Inhalt
zum selben Zweck prüfen. Die zwei Erstentwürfe getrennt halten und ihre Inhalte
nur im Umfang eines konkreten Änderungsauftrags bearbeiten.

## Änderungsgrenzen

Keine Commits ohne ausdrückliche Freigabe vor jedem Commit. Git-Initialisierung,
Remote-Erstellung, Push und echte PRs brauchen einen entsprechenden Auftrag.
Keine andere Lizenz, Automationen oder zusätzlichen Werkzeuge eigenmächtig hinzufügen.
Eine Anfrage oder Vorlage ist keine Ausführungserlaubnis.

Vor Änderungen an AGENTS.md oder Skills einen Rückweg sichern: vorhandene
Git-Historie oder Snapshot, solange kein Git besteht. Neue Dateien über ein
Manifest mit Inhaltshashes erfassen; beim Rückbau spätere Änderungen schützen.
Nach Änderungen an Agent-Konfiguration den eigenen Diff adversarial prüfen:
Erweitert eine Regel den Auftrag? Fehlt eine Freigabegrenze? Widersprechen sich
Skill und gemeinsame Regeln? Sind Links und Metadaten gültig?

## Nachweis und Arbeitsstand

Bei mehrschrittiger Arbeit eine kurze Aufgabenliste führen. Relevanten dauerhaften
Projektstand in README.md halten, Inhaltsänderungen beim betroffenen Dokument
nachvollziehbar machen. Vor Abschluss den Prüfmaßstab aus docs/README.md anwenden
und Ergebnisse sowie Grenzen nennen. Keine bestandene Prüfung ohne Beobachtung
behaupten; eine formale Prüfung belegt keine praktische Erprobung.
