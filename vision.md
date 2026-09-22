# Vision: AI Team Playbook

Deutsch (Standard) | [English](vision.en.md)

- Status: Entwurf
- Pflegeverantwortung: UNBEKANNT: noch nicht zugewiesen
- Inhaltlich geprüft: 2026-09-22 gegen den lokalen Projektstand
- Nächster Prüfanlass: vor der ersten Veröffentlichung oder bei einer Änderung des Projektziels
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

Projektlokale Skills führen Menschen und Agenten durch das Erstellen, Anpassen
und Ändern der Inhalte. Änderungsanfragen und Pull Requests verbinden Bedarf,
Entscheidung, Umsetzung und Prüfnachweis. Erfahrungen werden erst dann als solche
bezeichnet, wenn ihr Kontext und Ergebnis dokumentiert sind.

Die Bibliothek ergänzt `ki-agent-setup`, bleibt aber ein eigenständiges Projekt.
Teams übernehmen nur die Teile, die sie bewusst auswählen und für ihren Kontext
anpassen.

## Rollen

- Die Pflegeverantwortung hält Struktur, Status und Verweise der Bibliothek
  aktuell. Diese Rolle ist noch nicht zugewiesen.
- Inhaltsverantwortliche prüfen einzelne Prozesse und ihre Nachweise bei
  Änderungen oder praktischen Rückmeldungen.
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
- Zwei getrennte Erstentwürfe liegen unter `docs/entwuerfe/`.
- Vorlagen für Inhalte, Änderungsanfragen und Pull Requests liegen unter
  `docs/vorlagen/`.
- Drei projektlokale Skills unterstützen Erstellung, Anpassung sowie Anfragen
  und Pull Requests.
- Git ist mit dem Branch `main` initialisiert. Das öffentliche Remote
  [derivo/ai-team-playbook](https://github.com/derivo/ai-team-playbook) ist als
  `origin` eingerichtet. Die zweisprachige Grundlage bildet die erste
  Veröffentlichung; Pull Requests existieren noch nicht.
- Eine Lizenz und die Pflegeverantwortung sind noch nicht festgelegt.

Dieser Abschnitt ist eine Momentaufnahme. Bei der Wiederaufnahme müssen die
Aussagen gegen den tatsächlichen Projektstand geprüft werden.

## Ablauf bis zur ersten Veröffentlichung

### 1. Inhalt und Grenzen prüfen

Die beiden Erstentwürfe, Vorlagen, Skills und diese Vision gemeinsam prüfen.
Offene Änderungswünsche als lokale Änderungsanfragen erfassen. Akzeptanzkriterium:
Projektzweck, Zielgruppe, Abgrenzung und erste Inhalte widersprechen einander
nicht; verbleibende Streitpunkte sind ausdrücklich dokumentiert.

### 2. Pflege und Lizenz entscheiden

Eine menschliche Pflegeverantwortung benennen und eine Lizenz bewusst auswählen.
Die Entscheidung zur Lizenz darf nicht durch einen Agenten vorweggenommen werden.
Akzeptanzkriterium: Verantwortung und Lizenzentscheidung sind dokumentiert; die
gewählte Lizenzdatei existiert erst nach dieser Entscheidung.

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

1. AGENTS.md, vision.md, README.md und docs/README.md vollständig lesen.
2. Projektdateien und gegebenenfalls git status prüfen; nichts aus dieser
   Momentaufnahme ungeprüft übernehmen.
3. Vorhandene Änderungsanfragen und offene Entscheidungen suchen.
4. Den ersten unerledigten Schritt unter „Ablauf bis zur ersten
   Veröffentlichung“ benennen und nur dessen Voraussetzungen bearbeiten.
5. Keine Lizenz wählen, kein Git initialisieren, keinen Commit erstellen, kein
   Remote anlegen und nichts veröffentlichen, solange das nicht ausdrücklich
   beauftragt beziehungsweise freigegeben wurde.
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
Sie legt weder eine Lizenz noch eine technische Plattform jenseits der bereits
beschriebenen GitHub-Arbeitsweise fest. Sie behauptet keine Praxiserprobung und
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
