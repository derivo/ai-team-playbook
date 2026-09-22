# AI Team Playbook

Deutsch (Standard) | [English](README.en.md)

Eine öffentliche Bibliothek anpassbarer Prozesse, Standards und Vorlagen für die
Zusammenarbeit von Menschen und KI-Agenten.

Das Playbook macht gemeinsame Arbeitsweisen sichtbar, überprüfbar und
wiederverwendbar. Es ist kein allgemeingültiges Firmenhandbuch: Jedes Team
entscheidet selbst, welche Inhalte es übernimmt, anpasst und verbindlich macht.

## Prozessübersicht

| Prozess | Was wird geregelt? | Wann ist er hilfreich? | Anwendungsfall |
| --- | --- | --- | --- |
| [Zusammenarbeit von Menschen und KI-Agenten](docs/prozesse/zusammenarbeit-mensch-ki.md) | Aufgabenübernahme, Statuspflege, Übergaben, KI-Reviews und Nacharbeiten | Wenn mehrere Menschen mit eigenen KI-Agenten an gemeinsamen Änderungen arbeiten | [GitHub mit lokalen Claude-Clients](docs/anwendungsfaelle/teamprozess-mensch-ki-github.md) |
| [Lebenszyklus gemeinsam genutzter Anwendungen](docs/prozesse/anwendungs-lebenszyklus.md) | Idee, Einordnung, Versuch, Betriebsübernahme, regelmäßige Prüfung und Abschaltung | Wenn aus einer Idee eine gemeinsam genutzte und betreute Anwendung werden kann | [App-Lifecycle im Unternehmen](docs/anwendungsfaelle/gedankenspiel-app-lifecycle.md) |

Die Prozesse sind allgemein gültig und unabhängig von Werkzeugen und
Organisationen formuliert; das gilt ebenso für die Standards unten.
Anwendungsfälle zeigen, wie ein Prozess in einem konkreten Kontext ausgeprägt
sein kann. Alle Inhalte haben den Status Entwurf:
Es sind Vorschläge, deren praktische Erprobung noch nicht belegt ist.

## Standards

| Standard | Was wird geregelt? |
| --- | --- |
| [Freigabegrenzen für KI-Agenten](docs/standards/freigabegrenzen-fuer-agenten.md) | Was ein Agent selbstständig tun darf und was eine menschliche Freigabe braucht |
| [Nachweis statt Selbsteinschätzung](docs/standards/nachweis-statt-selbsteinschaetzung.md) | Fertig-Meldungen mit beobachteten Prüfergebnissen, Unbekanntes gekennzeichnet |
| [Daten und Vertraulichkeit bei KI-Nutzung](docs/standards/daten-und-vertraulichkeit.md) | Welche Daten an welche KI-Werkzeuge gehen dürfen, Schutz von Zugangsdaten |
| [Agent-Konfiguration als gepflegtes Artefakt](docs/standards/agent-konfiguration.md) | Regeln und Skills für Agenten versioniert im Projekt, mit Review und Rückweg |
| [Kennzeichnung von KI-Beiträgen](docs/standards/kennzeichnung-von-ki-beitraegen.md) | Wann und wie KI-Mitarbeit in Commits, Änderungsvorschlägen und Reviews sichtbar wird |

## Playbook verwenden

1. In der Prozessübersicht einen passenden Ausgangspunkt auswählen.
2. Problem, Rollen, Voraussetzungen und Grenzen des Prozesses lesen.
3. Begriffe und Ablauf an den eigenen Teamkontext anpassen.
4. Im Team entscheiden, welche Teile verbindlich gelten.
5. Erfahrungen und Änderungsbedarf nachvollziehbar dokumentieren.

Die [Vision](vision.md) beschreibt Zweck, Zielbild und Grundsätze des Projekts.
Aufbau, Statusmodell und Pflege der Inhalte stehen in der
[Dokumentstruktur](docs/README.md).

## Vorlagen und Skills

| Hilfsmittel | Zweck |
| --- | --- |
| [Inhaltsvorlage](docs/vorlagen/inhalt.md) | Einen neuen Prozess oder Standard einheitlich strukturieren |
| [Änderungsanfrage](docs/vorlagen/aenderungsanfrage.md) | Problem, Ziel, Umfang und Entscheidung nachvollziehbar festhalten |
| [Pull-Request-Vorlage](docs/vorlagen/pull-request.md) | Änderung und Prüfnachweise für ein Review zusammenfassen |
| [Projektlokale Skills](AGENTS.md#passenden-skill-wählen) | KI-Agenten beim Erstellen, Anpassen und Prüfen von Inhalten anleiten |

## Sprachen

Deutsch ist die Standardsprache und verwendet Dateinamen ohne Sprachsuffix.
Englische Fassungen liegen jeweils daneben und tragen `.en.md`. Beide Fassungen
werden gemeinsam gepflegt und verlinken einander.

## Beitragen

Vor einem neuen Beitrag prüfen, ob bereits ein Inhalt mit demselben Zweck
existiert. Ein Änderungsvorschlag soll das konkrete Problem, das gewünschte
Ergebnis und einen überprüfbaren Abschluss beschreiben. Öffentliche Inhalte
werden immer gemeinsam auf Deutsch und Englisch geändert.

Die [Projektregeln](AGENTS.md) enthalten die vollständigen Pflege- und
Prüfvorgaben.

## Lizenz

Dokumentation, Prozesse, Vorlagen und Skills stehen unter
[CC BY 4.0](LICENSES/CC-BY-4.0.txt). Software und ausführbare Skripte stehen unter
[Apache-2.0](LICENSES/Apache-2.0.txt). Die genaue Zuordnung und Hinweise zur
Namensnennung stehen in der [Lizenzübersicht](LICENSE.md).
