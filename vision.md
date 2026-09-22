# Vision: AI Team Playbook

Deutsch (Standard) | [English](vision.en.md)

- Status: Entwurf
- Pflegeverantwortung: Maintainer-Team (prüft Änderungen im Review)
- Inhaltlich geprüft: 2026-09-22 gegen den lokalen Projektstand
- Nächster Prüfanlass: vor der Startversion oder bei einer Änderung des Projektziels
- Erprobungsnachweis: Keiner; die Bibliothek ist noch nicht praktisch erprobt.
- Verbindlichkeit: Jedes übernehmende Team entscheidet selbst.

## Problem

Teams entwickeln eigene Regeln für die Zusammenarbeit von Menschen und
KI-Agenten häufig in einzelnen Chats, lokalen Dateien oder voneinander getrennten
Projekten. Entscheidungen, Vorlagen und Lernerfahrungen gehen dadurch verloren
oder werden mehrfach erarbeitet. Nach einer Unterbrechung ist oft unklar, was
bereits vorbereitet wurde, welche Entscheidungen noch fehlen und welcher Schritt
als Nächstes sinnvoll ist.

Das AI Team Playbook soll dafür eine öffentliche, nachvollziehbar gepflegte
Bibliothek schaffen. Es sammelt anpassbare Standards, Prozesse und Workflows,
ohne sie automatisch zu verbindlichen Unternehmensregeln zu erklären.

## Zielgruppe

Die Bibliothek richtet sich an Teams, die Menschen und KI-Agenten gemeinsam an
Software, Dokumentation oder betrieblichen Abläufen arbeiten lassen. Sie soll
sowohl Menschen als auch Agenten ermöglichen,

- einen passenden Prozess schnell zu finden,
- seinen Reifegrad und seine Grenzen zu erkennen,
- ihn kontrolliert an den eigenen Kontext anzupassen und
- Änderungen mit überprüfbaren Gründen und Nachweisen weiterzugeben.

## Zielbild

Das Repository enthält eine kleine, verständliche Sammlung eigenständiger
Playbook-Inhalte. Jeder Inhalt beschreibt Problem, Zielgruppe, Rollen, Ablauf,
direkt nutzbare Vorlagen und Grenzen. Der Status zeigt, ob ein Inhalt ein Entwurf,
in einem dokumentierten Kontext erprobt oder durch einen Nachfolger abgelöst ist.

Prozesse und Standards sind allgemein gültig und unabhängig von Werkzeugen,
Agenten und Organisationen formuliert. Aus ihnen werden reale Anwendungsfälle
abgeleitet, etwa die Arbeit mit GitHub in einem Unternehmen, in dem Kollegen
eigene Claude-Clients nutzen. Ein Anwendungsfall verweist auf seinen Prozess und
beschreibt nur, was in seinem Kontext konkret anders oder genauer geregelt ist.

Projektlokale Skills führen Menschen und Agenten durch das Erstellen, Anpassen
und Ändern der Inhalte. Änderungsanfragen und Pull Requests verbinden Bedarf,
Entscheidung, Umsetzung und Prüfnachweis. Erfahrungen werden erst dann als solche
bezeichnet, wenn ihr Kontext und Ergebnis dokumentiert sind.

Die Bibliothek ergänzt `ki-agent-setup`, bleibt aber ein eigenständiges Projekt.
Teams übernehmen nur die Teile, die sie bewusst auswählen und für ihren Kontext
anpassen.

## Rollen

- Das Maintainer-Team hält Struktur, Status und Verweise der Bibliothek
  aktuell und prüft Änderungen im Review. In einem Fork oder einer Kopie
  benennt das übernehmende Team eigene Zuständige.
- Inhaltsverantwortliche prüfen einzelne Prozesse und ihre Nachweise bei
  Änderungen oder praktischen Rückmeldungen. Derzeit übernimmt das
  Maintainer-Team diese Rolle.
- Beitragende beschreiben Änderungsbedarf nachvollziehbar und liefern passende
  Prüfnachweise.
- Übernehmende Teams entscheiden selbst über Anpassung und Verbindlichkeit.
- KI-Agenten unterstützen Recherche, Erstellung und Prüfung, treffen aber keine
  organisatorischen Entscheidungen anstelle eines Menschen.

## Aktueller Stand

Am 2026-09-22 wurde der folgende lokale Stand geprüft:

- Der Projektordner `/Users/dennis/code/ai-team-playbook` besteht.
- [Projektübersicht](README.md), [Projektregeln](AGENTS.md) und
  [Dokumentstruktur](docs/README.md) sind angelegt.
- Zwei allgemeine Prozesse liegen unter `docs/prozesse/`, fünf Standards unter
  `docs/standards/`. Die beiden übernommenen Erstentwürfe liegen als Anwendungsfälle unter
  `docs/anwendungsfaelle/` und verweisen auf ihren Prozess.
- Vorlagen für Inhalte, Änderungsanfragen und Pull Requests liegen unter
  `docs/vorlagen/`.
- Drei projektlokale Skills unterstützen Erstellung, Anpassung sowie Anfragen
  und Pull Requests.
- Git ist mit dem Branch `main` initialisiert. Das öffentliche Remote
  [derivo/ai-team-playbook](https://github.com/derivo/ai-team-playbook) ist als
  `origin` eingerichtet. Die zweisprachige Grundlage bildet die erste
  Veröffentlichung; Pull Requests existieren noch nicht.
- Die Lizenzierung ist festgelegt: redaktionelle Inhalte verwenden `CC-BY-4.0`,
  Software und ausführbare Skripte `Apache-2.0`. Die Pflegeverantwortung liegt
  beim Maintainer-Team.

Dieser Abschnitt ist eine Momentaufnahme. Bei der Wiederaufnahme müssen die
Aussagen gegen den tatsächlichen Projektstand geprüft werden.

## Ablauf bis zur Startversion

### 1. Inhalt und Grenzen prüfen

Status: am 2026-09-22 geprüft und umgesetzt.

Die beiden Erstentwürfe, Vorlagen, Skills und diese Vision gemeinsam prüfen.
Offene Änderungswünsche erfassen. Akzeptanzkriterium:
Projektzweck, Zielgruppe, Abgrenzung und erste Inhalte widersprechen einander
nicht; verbleibende Streitpunkte sind ausdrücklich dokumentiert.

Ergebnis: Die Entwürfe waren an ein Unternehmen und bestimmte Werkzeuge
gebunden. Entschieden wurde, Prozesse allgemein gültig zu formulieren und die
Entwürfe als Anwendungsfälle zu führen. Bis zur Startversion werden Änderungen
direkt im Repository vorgenommen, danach als GitHub-Issues erfasst. Neue Inhalte
pflegt standardmäßig das Maintainer-Team; es übernimmt derzeit auch die Rolle der
Inhaltsverantwortlichen. Die Startversion ist fertig, wenn das Maintainer-Team
sie ausdrücklich für fertig erklärt.

### 2. Pflege und Lizenz entscheiden

Status: am 2026-09-22 umgesetzt.

Die Pflegeverantwortung liegt beim Maintainer-Team. Die Lizenzierung wurde am
2026-09-22 mit `CC-BY-4.0` für redaktionelle Inhalte und `Apache-2.0` für Software
festgelegt. Akzeptanzkriterium: Die Verantwortung ist dokumentiert und neue
Dateien folgen der festgelegten Lizenzzuordnung.

### 3. Versionsverwaltung vorbereiten

Status: am 2026-09-22 für die erste Veröffentlichung umgesetzt.

Nach ausdrücklichem Auftrag Git initialisieren, den lokalen Zustand prüfen und
vor einem Commit eine gesonderte Freigabe einholen. Akzeptanzkriterium: Der
vorgesehene Commit enthält ausschließlich geprüfte Projektdateien und keine
Secrets oder temporären Arbeitsdateien.

### 4. Veröffentlichung vorbereiten

Status: am 2026-09-22 mit dem öffentlichen Repository
`derivo/ai-team-playbook` umgesetzt.

Nach ausdrücklichem Auftrag ein öffentliches Remote einrichten. Vor dem Push
Repository-Name, Sichtbarkeit, Standardbranch, README, Lizenz und Links prüfen.
Akzeptanzkriterium: Das Remote entspricht den getroffenen Entscheidungen und der
lokale Branch ist eindeutig zugeordnet. Push und Veröffentlichung erfolgen nur
im ausdrücklich freigegebenen Umfang.

### 5. Einen Inhalt erproben

Status: am 2026-09-22 vorbereitet, siehe
[Erprobungsplan](docs/erprobungen/teamprozess-mensch-ki-github.md); Team,
Repository, Teilnehmende und Zeitraum sind noch festzulegen.

Ein Team wählt einen Entwurf aus, passt ihn an einen benannten Kontext an und
dokumentiert Zeitraum, Vorgehen, Ergebnis und Grenzen. Akzeptanzkriterium: Eine
unbeteiligte Person kann nachvollziehen, was erprobt wurde und welche Aussagen
der Nachweis trägt. Erst dann darf der Inhalt den Status `erprobt` erhalten.

### 6. Pflegezyklus etablieren

Rückmeldungen als Änderungsanfragen erfassen, Änderungen per Pull Request prüfen
und abgelöste Inhalte mit Begründung und Nachfolger erhalten. Akzeptanzkriterium:
Für jeden aktiven Inhalt sind Pflegeverantwortung und nächster Prüfanlass sichtbar.

## Vorlage für die Wiederaufnahme

Eine neue Session beginnt mit diesem Block:

```text
Ziel: Die Arbeit am AI Team Playbook am ersten unerledigten Schritt fortsetzen.
Projekt: /Users/dennis/code/ai-team-playbook

1. AGENTS.md, vision.md, vision.en.md, README.md und docs/README.md vollständig
   lesen.
2. Projektdateien und gegebenenfalls git status prüfen; nichts aus dieser
   Momentaufnahme ungeprüft übernehmen.
3. Vorhandene Änderungsanfragen und offene Entscheidungen suchen.
4. Den ersten unerledigten Schritt unter „Ablauf bis zur Startversion“
   benennen und nur dessen Voraussetzungen bearbeiten.
5. Keine andere Lizenz wählen, keinen Commit erstellen, nicht pushen und nichts
   veröffentlichen, solange das nicht ausdrücklich beauftragt beziehungsweise
   freigegeben wurde.
6. Nach der Arbeit vision.md und vision.en.md nur dort aktualisieren, wo sich der
   belegte Zustand, eine Entscheidung oder der nächste Schritt tatsächlich
   geändert hat.
```

## Vorlagen

- [Inhaltsvorlage](docs/vorlagen/inhalt.md)
- [Vorlage für Änderungsanfragen](docs/vorlagen/aenderungsanfrage.md)
- [Vorlage für Pull Requests](docs/vorlagen/pull-request.md)

## Grenzen

Die Vision ist kein verbindlicher Zeitplan und keine Veröffentlichungserlaubnis.
Sie legt keine technische Plattform jenseits der bereits beschriebenen
GitHub-Arbeitsweise fest; die Lizenzierung regelt die [Lizenzübersicht](LICENSE.md). Sie behauptet keine Praxiserprobung und
ersetzt keine konkrete Änderungsanfrage.

Die Bibliothek soll klein und anpassbar bleiben. Neue Inhalte entstehen aus einem
konkreten Bedarf; Automationen, Integrationen und zusätzliche Varianten werden
nicht vorsorglich angelegt.

## Quellen

- Der am 2026-09-22 beobachtete lokale Projektstand
- [Projektübersicht](README.md)
- [Projektregeln](AGENTS.md)
- [Dokumentstruktur und Pflege](docs/README.md)
- Der Auftrag, eine nahtlose spätere Wiederaufnahme zu ermöglichen

## Änderungsverlauf

- 2026-09-22: Erster Entwurf mit Zielbild, geprüftem Ausgangsstand,
  Veröffentlichungspfad und Wiederaufnahmevorlage angelegt.
- 2026-09-22: Lizenzierung (`CC-BY-4.0` für redaktionelle Inhalte, `Apache-2.0`
  für Software) festgehalten und das Maintainer-Team als Pflegeverantwortung
  eingetragen; Schritt 2 als umgesetzt markiert.
- 2026-09-22: Schritt 1 umgesetzt: allgemeine Prozesse unter `docs/prozesse/`
  angelegt, Erstentwürfe als Anwendungsfälle nach `docs/anwendungsfaelle/`
  verschoben, Ablauf auf die Startversion ausgerichtet.
- 2026-09-22: Maintainer-Team als Standard-Pflegeverantwortung für neue Inhalte
  in Vorlage, Dokumentstruktur und Skill festgelegt.
- 2026-09-22: Startversion und Inhaltsverantwortung entschieden; Erprobung des
  Teamprozesses vorbereitet.
- 2026-09-22: Fünf Standards zu Freigabegrenzen, Nachweisen, Daten und
  Vertraulichkeit, Agent-Konfiguration und Kennzeichnung von KI-Beiträgen unter
  `docs/standards/` angelegt.
