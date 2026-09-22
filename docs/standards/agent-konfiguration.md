# Standard: Agent-Konfiguration als gepflegtes Artefakt

Deutsch (Standard) | [English](agent-konfiguration.en.md)

- Status: Entwurf
- Pflegeverantwortung: Maintainer-Team (prüft Änderungen im Review)
- Inhaltlich geprüft: 2026-09-22 gegen die Projektregeln dieses Repositorys; keine Praxiserprobung belegt.
- Nächster Prüfanlass: vor einer Übernahme ins Team und bei praktischen Rückmeldungen
- Erprobungsnachweis: Keiner; nicht als erprobt ausgewiesen.
- Verbindlichkeit: Entscheidung des übernehmenden Teams.
- Anwendungsfälle: Noch keine.

Pflege und Formate: [Dokumentstruktur](../README.md).

## Problem

Wie sich ein KI-Agent in einem Projekt verhält, hängt von seinen Anweisungen ab:
Regeldateien, Skills, Einstellungen. Liegen sie nur lokal bei Einzelnen, arbeiten
Agenten im selben Projekt nach unterschiedlichen Regeln. Ungeprüfte Änderungen
können Freigabegrenzen aufweichen, ohne dass es jemand bemerkt.

## Zielgruppe

Teams, in denen mehrere Personen KI-Agenten im selben Projekt einsetzen.

## Rollen

- **Pflegeverantwortliche:** halten die Projektkonfiguration aktuell und prüfen
  Änderungen daran.
- **Beitragende:** schlagen Änderungen an der Konfiguration wie an anderem Inhalt
  vor.
- **KI-Agent:** liest die Projektkonfiguration und ändert sie nur auf Auftrag.

## Ablauf

### 1. Konfiguration im Projekt ablegen

Projektregeln für Agenten liegen versioniert im Repository, zum Beispiel in einer
`AGENTS.md`. Werkzeugspezifische Dateien verweisen auf diese gemeinsame Quelle,
statt Regeln zu kopieren. Projektspezifische Skills liegen ebenfalls im
Repository.

### 2. Gemeinsame und persönliche Regeln trennen

Persönliche Einstellungen bleiben lokal. Was für alle im Projekt gilt, steht in
der Projektkonfiguration. Bei Widerspruch geht die Projektregel vor, sofern das
Team nichts anderes festlegt.

### 3. Änderungen reviewen

Änderungen an Regeln, Skills oder Einstellungen laufen durch dasselbe Review wie
andere Änderungen. Der Review prüft gezielt:

- Erweitert eine Regel den Auftrag oder die Befugnisse eines Agenten?
- Fehlt eine Freigabegrenze oder wird eine aufgeweicht?
- Widersprechen sich Regeln, Skills und gemeinsame Vorgaben?
- Sind Verweise und Metadaten gültig?

### 4. Rückweg sichern

Vor einer Änderung existiert ein Rückweg, in der Regel die Versionshistorie. Eine
Änderung an der Konfiguration wird einzeln nachvollziehbar gehalten, nicht mit
unabhängigen Inhaltsänderungen vermischt.

## Vorlagen

```text
Minimaler Verweis in einer werkzeugspezifischen Datei:
@AGENTS.md
```

Die Syntax für Verweise hängt vom Werkzeug ab.

## Grenzen

- Der Standard legt keine Inhalte der Regeln fest, nur ihren Umgang.
- Nicht jedes Werkzeug unterstützt Verweise zwischen Dateien; dann ist eine
  gepflegte Kopie mit Hinweis auf die Quelle der Kompromiss.
- Anpassungspunkte: Dateinamen, Ablage der Skills, Tiefe des Reviews.

## Quellen

- Abgeleitet aus den [Projektregeln](../../AGENTS.md) dieses Repositorys, dessen
  `CLAUDE.md` auf die `AGENTS.md` verweist.
- Vorschlag ohne belegte Praxiserprobung.

## Änderungsverlauf

- 2026-09-22: Als Standard angelegt.
