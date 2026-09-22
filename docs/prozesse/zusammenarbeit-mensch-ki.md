# Zusammenarbeit von Menschen und KI-Agenten an gemeinsamen Änderungen

Deutsch (Standard) | [English](zusammenarbeit-mensch-ki.en.md)

- Status: Entwurf
- Pflegeverantwortung: Maintainer-Team (prüft Änderungen im Review)
- Inhaltlich geprüft: 2026-09-22 aus dem Anwendungsfall abgeleitet; keine Praxiserprobung belegt.
- Nächster Prüfanlass: vor einer Übernahme ins Team und bei praktischen Rückmeldungen
- Erprobungsnachweis: Keiner; nicht als erprobt ausgewiesen.
- Verbindlichkeit: Entscheidung des übernehmenden Teams.
- Anwendungsfälle: [Teamprozess mit GitHub und lokalen Claude-Clients](../anwendungsfaelle/teamprozess-mensch-ki-github.md)

Pflege und Formate: [Dokumentstruktur](../README.md).

## Problem

Wenn mehrere Menschen jeweils eigene KI-Agenten an gemeinsamen Änderungen
arbeiten lassen, ist oft unklar, wer eine Aufgabe verantwortet, ob bereits
jemand daran arbeitet, ob ein Agent noch läuft und wer als Nächstes handeln muss.
Doppelte Umsetzungen, liegengebliebene Reviews und vergessene Nacharbeiten sind
die Folge.

## Zielgruppe

Teams, die Änderungen an Code, Dokumentation oder anderen versionierten Inhalten
gemeinsam erarbeiten und dabei KI-Agenten einsetzen. Vorausgesetzt werden eine
gemeinsame Aufgabenverwaltung und ein Verfahren für Änderungsvorschläge mit
Review, zum Beispiel Pull oder Merge Requests. Werkzeuge und Agenten sind frei
wählbar.

## Rollen

- **Verantwortlicher Mensch:** besitzt die Aufgabe, beauftragt den Agenten,
  klärt Anforderungen und gibt Ergebnisse zur Prüfung frei. Jede Aufgabe hat
  genau einen verantwortlichen Menschen, auch wenn ein Agent sie umsetzt.
- **Ausführender Agent:** setzt die Aufgabe im beauftragten Umfang um und hält
  den Stand aktuell, soweit das Team ihm diese Pflege überträgt.
- **Reviewer:** ein benannter Mensch, der den Änderungsvorschlag prüft und
  freigibt. Automatische Reviews liefern Hinweise; die menschliche Freigabe
  bleibt erforderlich.
- **Review-Agent:** ein KI-Agent, der einen Änderungsvorschlag prüft. Jeder Lauf
  hat einen verantwortlichen Menschen.

## Ablauf

### 1. Aufgabe übernehmen

Vor Arbeitsbeginn die Aufgabe in der gemeinsamen Aufgabenverwaltung anlegen oder
eine bestehende verwenden. Ziel und Fertig-Kriterium kurz beschreiben. Prüfen, ob
bereits jemand daran arbeitet. Der verantwortliche Mensch trägt sich ein und
setzt den Stand auf **In Arbeit**.

Abschluss: Die Aufgabe nennt Verantwortlichen, Ziel, Fertig-Kriterium und Stand.

### 2. Agent beauftragen

Der verantwortliche Mensch übergibt dem Agenten Aufgabe, Ziel und Grenzen des
Auftrags. Der Agent prüft vorhandene verknüpfte Änderungsvorschläge, damit keine
doppelte Umsetzung entsteht. Unklare Anforderungen klärt der verantwortliche
Mensch.

### 3. Arbeit früh sichtbar machen

Sobald erste Änderungen vorliegen, wird ein als Entwurf gekennzeichneter
Änderungsvorschlag angelegt und mit der Aufgabe verknüpft. Ein Entwurf zeigt
laufende Arbeit; er ist noch keine Aufforderung zum Review.

### 4. Stand aktuell halten

Bei Beginn, Pause, Blockade und Übergabe den Statusblock der Aufgabe
aktualisieren. Bei einer Blockade festhalten, was fehlt und wer als Nächstes
handeln muss. Datum und Uhrzeit der Aktualisierung mitführen: Ein alter Eintrag
„In Arbeit“ beweist nicht, dass ein Agent noch läuft.

### 5. Review übergeben

Nach den vereinbarten Prüfungen kontrolliert der verantwortliche Mensch Ergebnis
und Prüfnachweise, markiert den Änderungsvorschlag als reviewbereit und benennt
einen konkreten Reviewer. Die Aufgabe steht auf **Wartet auf Review**,
einschließlich Reviewer und nächstem Schritt.

Hinweise automatischer Reviews werden bearbeitet oder begründet verworfen. Bei
Änderungswünschen geht der nächste Schritt an den Verantwortlichen zurück; nach
der Überarbeitung wird erneut geprüft und ein neues Review angefordert.

### 6. KI-Reviews nachverfolgen

Der Aufgabenstand bleibt bei der Aufgabe, der Review-Eintrag beim
Änderungsvorschlag, weil er sich auf einen bestimmten Versionsstand bezieht. Die
Aufgabe verweist auf den aktuellen Review-Eintrag.

- **Vor dem Start:** prüfen, ob für diesen Versionsstand bereits ein Review läuft.
  Einen Review-Eintrag mit verantwortlichem Menschen, Agent/Sitzung, geprüftem
  Versionsstand, Startzeit und erwarteter nächster Rückmeldung anlegen. Ein
  zusätzlicher unabhängiger Review wird nur bewusst gestartet und kenntlich
  gemacht.
- **Während des Reviews:** den Eintrag regelmäßig mit letzter Rückmeldung und
  Zwischenstand aktualisieren. Das Intervall legt das Team fest.
- **Ausbleibende Rückmeldung:** Ein abgestürzter Agent kann seinen Ausfall nicht
  zuverlässig selbst melden. Eine vom Agenten unabhängige Überwachung oder, ohne
  sie, der verantwortliche Mensch prüft den Lauf zum vereinbarten Zeitpunkt. Eine
  überfällige Rückmeldung heißt „Zustand unklar“, nicht automatisch Abbruch.
- **Abbruch und Ersatzlauf:** Vor einem Ersatzlauf klären, ob der bisherige Lauf
  noch arbeitet. Befunde und offene Prüfpunkte bleiben im bisherigen Eintrag; der
  neue Lauf verweist darauf. Ein abgebrochener Lauf gilt nicht als abgeschlossener
  Review.
- **Abschluss:** Das Ergebnis wird verlinkt, mit geprüftem Versionsstand und
  Angabe, ob der Review vollständig war. Neue Änderungen sind durch einen älteren
  Review nicht automatisch abgedeckt.

### 7. Abschließen und Nacharbeiten erfassen

Nach menschlicher Freigabe und erfüllten Projektprüfungen wird die Änderung
übernommen. Vor dem Schließen der Aufgabe werden alle erkannten offenen
Nacharbeiten als eigene Aufgaben angelegt, jeweils mit offenem Punkt, Kontext und
Grund. Ursprüngliche Aufgabe und Nacharbeiten verweisen gegenseitig aufeinander.
Eine als nicht erforderlich eingestufte Nacharbeit wird mit Begründung
geschlossen, nicht gelöscht.

Abschluss: Die Änderung ist übernommen, die Aufgabe geschlossen, und jede
Nacharbeit ist als verknüpfte Aufgabe sichtbar.

## Vorlagen

### Statusangaben

| Stand | Bedeutung |
|---|---|
| Offen | Noch nicht übernommen |
| In Arbeit | Ein Mensch bearbeitet die Aufgabe, gegebenenfalls mit Agent |
| Pausiert | Arbeit bewusst unterbrochen |
| Blockiert | Eine konkrete Voraussetzung oder Entscheidung fehlt |
| Wartet auf Review | Ein benannter Reviewer ist als Nächstes dran |
| In Überarbeitung | Der Verantwortliche bearbeitet Review-Rückmeldungen |
| Erledigt | Änderung übernommen und Aufgabe abgeschlossen |

### Statusblock der Aufgabe

```text
Verantwortlich: [Name]
Agent: [Agent und Ort der Ausführung]
Stand: [Statusangabe]
Änderungsvorschlag: [Verweis oder „Noch keiner“]
KI-Review: [Verweis auf den Review-Eintrag oder „Noch nicht gestartet“]
Nächster Schritt: [Person und Handlung]
Blockade: [Ursache oder „Keine“]
Zuletzt aktualisiert: [Datum und Uhrzeit]
```

### Review-Eintrag am Änderungsvorschlag

```text
Verantwortlich: [Name]
Agent/Sitzung: [eindeutige Bezeichnung des Review-Laufs]
Geprüfter Versionsstand: [Kennung]
Review-Stand: Läuft / Blockiert / Zustand prüfen / Abgebrochen / Fertig
Gestartet: [Datum und Uhrzeit]
Letzte Rückmeldung: [Datum und Uhrzeit]
Nächste Rückmeldung erwartet bis: [Datum und Uhrzeit]
Zwischenstand: [geprüfte Bereiche, Befunde, offene Prüfpunkte]
Nächster Schritt und zuständige Person: [...]
Ergebnis oder vorheriger Lauf: [Verweis, soweit vorhanden]
```

## Grenzen

- Der Prozess setzt eine gemeinsame Aufgabenverwaltung und ein Review-Verfahren
  voraus; er ersetzt keine Projektprüfungen oder Freigaberegeln.
- Überwachung, Benachrichtigung und die Vergabe von Review-Läufen an genau einen
  Agenten sind Anpassungspunkte. Vorlagen und Statusangaben allein stellen diese
  Funktionen nicht bereit.
- Ohne technische Vergabe stimmen sich die Verantwortlichen vor einem Review-Start
  ab.
- Anpassungspunkte: Statusnamen, Rückmeldeintervall, Ort des Statusblocks,
  optionale Labels zum Filtern.
- Erfolgskriterium für eine Erprobung: Eine unbeteiligte Person erkennt anhand
  der Aufgabe ohne Nachfragen den Verantwortlichen, den Änderungsvorschlag, den
  Stand und die nächste zuständige Person.

## Quellen

- Abgeleitet aus dem Anwendungsfall
  [Teamprozess mit GitHub und lokalen Claude-Clients](../anwendungsfaelle/teamprozess-mensch-ki-github.md).
- Vorschlag ohne belegte Praxiserprobung.

## Änderungsverlauf

- 2026-09-22: Als werkzeugunabhängiger Prozess aus dem Anwendungsfall abgeleitet.
