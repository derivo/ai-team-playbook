# Standard: Daten und Vertraulichkeit bei KI-Nutzung

Deutsch (Standard) | [English](daten-und-vertraulichkeit.en.md)

- Status: Entwurf
- Pflegeverantwortung: Maintainer-Team (prüft Änderungen im Review)
- Inhaltlich geprüft: 2026-09-22 als Vorschlag verfasst; keine Praxiserprobung belegt.
- Nächster Prüfanlass: vor einer Übernahme ins Team und bei praktischen Rückmeldungen
- Erprobungsnachweis: Keiner; nicht als erprobt ausgewiesen.
- Verbindlichkeit: Entscheidung des übernehmenden Teams.
- Anwendungsfälle: Noch keine.

Pflege und Formate: [Dokumentstruktur](../README.md).

## Problem

Wer mit KI-Werkzeugen arbeitet, gibt ihnen Inhalte: Code, Dokumente,
Kundendaten, Zugangsdaten in Konfigurationsdateien. Ohne klare Regeln ist unklar,
welche Daten an welches Werkzeug gehen dürfen. Vertrauliche oder
personenbezogene Daten können so ungewollt an Dritte gelangen.

## Zielgruppe

Teams und Organisationen, die KI-Werkzeuge mit Zugriff auf eigene oder fremde
Daten nutzen. Der Standard gibt die Struktur vor; die konkreten Datenklassen und
Werkzeuge legt das übernehmende Team fest.

## Rollen

- **Team:** legt Datenklassen und freigegebene Werkzeuge fest.
- **Zuständige Fachstellen** (etwa Datenschutz oder IT-Sicherheit): werden bei
  der Festlegung und bei Zweifeln einbezogen.
- **Nutzende:** prüfen vor der Weitergabe an ein Werkzeug, welche Datenklasse
  betroffen ist.
- **KI-Agent:** gibt Daten nur im Rahmen der freigegebenen Werkzeuge weiter und
  meldet erkannte Zugangsdaten oder personenbezogene Daten.

## Ablauf

### 1. Datenklassen festlegen

Das Team legt wenige, verständliche Klassen fest, zum Beispiel: öffentlich,
intern, vertraulich, personenbezogen, Zugangsdaten.

### 2. Werkzeuge zuordnen

Für jedes eingesetzte KI-Werkzeug wird festgehalten, für welche Datenklassen es
freigegeben ist, wo die Daten verarbeitet werden und ob sie gespeichert oder für
Training verwendet werden können. Grundlage sind die geprüften Bedingungen des
Anbieters, nicht Annahmen.

### 3. Vor der Weitergabe prüfen

Vor dem Einfügen oder Freigeben von Inhalten prüfen, ob die Datenklasse für das
Werkzeug freigegeben ist. Im Zweifel nicht weitergeben und die zuständige Stelle
fragen.

### 4. Zugangsdaten schützen

Zugangsdaten gehören nicht in Prompts, Code, Dokumentation oder
Versionsverwaltung, sondern in dafür vorgesehene Ablagen wie Umgebungsvariablen
oder Secret-Speicher. Änderungen werden vor einem Commit auf Zugangsdaten und
echte Personendaten geprüft. Ein versehentlich weitergegebenes Geheimnis wird
ersetzt, nicht nur gelöscht.

### 5. Vorfälle melden

Gelangen Daten an ein nicht freigegebenes Werkzeug, wird das an die zuständige
Stelle gemeldet.

## Vorlagen

| Werkzeug | Freigegebene Datenklassen | Verarbeitungsort | Speicherung/Training | Geprüft am |
|---|---|---|---|---|
| [Name] | [z. B. öffentlich, intern] | [Region/Anbieter] | [laut geprüften Bedingungen] | [Datum] |

## Grenzen

- Der Standard ist keine Rechtsberatung und ersetzt keine rechtlichen,
  vertraglichen oder datenschutzrechtlichen Vorgaben.
- Er enthält bewusst keine konkrete Zuordnung von Werkzeugen, weil diese vom
  Anbieter, Vertrag und Kontext abhängt.
- Anpassungspunkte: Datenklassen, Werkzeugliste, zuständige Stellen,
  Meldeweg bei Vorfällen.

## Quellen

- Vorschlag ohne belegte Praxiserprobung. Die Regel zu Zugangsdaten entspricht
  dem Prüfmaßstab der [Dokumentstruktur](../README.md) dieses Repositorys.

## Änderungsverlauf

- 2026-09-22: Als Standard angelegt.
