# Erprobung: Teamprozess mit GitHub und lokalen Claude-Clients

Deutsch (Standard) | [English](teamprozess-mensch-ki-github.en.md)

- Stand: Vorbereitet
- Pflegeverantwortung: Maintainer-Team (prüft Änderungen im Review)
- Erprobter Anwendungsfall: [Teamprozess mit GitHub und lokalen Claude-Clients](../anwendungsfaelle/teamprozess-mensch-ki-github.md)
- Allgemeiner Prozess: [Zusammenarbeit von Menschen und KI-Agenten](../prozesse/zusammenarbeit-mensch-ki.md)
- Zeitraum: UNBEKANNT: Beginn und Ende
- Ergebnis: Noch keines; bis zur Auswertung bleiben beide Inhalte im Status Entwurf.

Pflege und Formate: [Dokumentstruktur](../README.md).

## Ziel und Fragestellung

Die Erprobung prüft, ob der Anwendungsfall in einem realen Team trägt:

1. Erkennt eine unbeteiligte Person allein anhand des Issues den
   Verantwortlichen, den zugehörigen PR, den Arbeitsstand und die nächste
   zuständige Person?
2. Wird ein unterbrochener KI-Review erkannt, und lässt sich sein bisheriger
   Stand vor einem Ersatzlauf nachvollziehen?
3. Ist der Pflegeaufwand für Statusblock und Review-Eintrag im Alltag tragbar?

Die Fragen 1 und 2 stammen aus dem Abschnitt „Einführung“ des Anwendungsfalls.
Frage 3 ergänzt den Aufwand, der für eine Übernahme ins Team entscheidend ist.

## Kontext

- Team: UNBEKANNT: Team oder Organisationseinheit
- Repository: UNBEKANNT: GitHub-Repository, in dem erprobt wird
- Teilnehmende: UNBEKANNT: zwei Personen mit eigenem lokalem Claude Code
- Unbeteiligte Person für die Auswertung: UNBEKANNT: Person, die weder Aufgabe
  noch Review bearbeitet
- Aufgabe: UNBEKANNT: eine echte, überschaubare Änderung mit Review

Namen realer Personen nur mit deren Einverständnis in diesem öffentlichen
Repository eintragen; sonst Rollen verwenden.

## Vorbereitung

- [ ] Team, Repository, Teilnehmende und unbeteiligte Person festlegen.
- [ ] Zeitraum festlegen; zwei bis vier Wochen sind ein Vorschlag, kein Erfahrungswert.
- [ ] Eine Aufgabe auswählen, die einen PR und ein Review erfordert.
- [ ] Anwendungsfall mit allen Teilnehmenden lesen und Abweichungen für das Team
      vorab notieren, etwa Statusnamen oder Rückmeldeintervall.
- [ ] Statusblock und Review-Eintrag aus dem Anwendungsfall bereitlegen. Statuspflege
      und Übernahme erfolgen manuell; Labels, Automationen und Überwachung werden
      für die Erprobung nicht eingerichtet.
- [ ] Vereinbaren, wer die Beobachtungen unten festhält.

## Ablauf

### Szenario A: Aufgabe von der Übernahme bis zum Abschluss

Die Teilnehmenden bearbeiten die Aufgabe nach den Schritten 1 bis 6 des
Anwendungsfalls: Issue übernehmen, Claude beauftragen, Draft-PR anlegen, Status
pflegen, Review übergeben, abschließen und Nacharbeiten als Issues erfassen.

Mindestens einmal während der Arbeit – etwa bei einer Pause oder Übergabe – und
einmal nach dem Abschluss liest die unbeteiligte Person nur das Issue und
beantwortet ohne Nachfragen Frage 1. Die Antworten werden mit dem tatsächlichen
Stand verglichen.

### Szenario B: Unterbrochener KI-Review

Ein KI-Review wird nach dem Abschnitt „KI-Reviews sichtbar übernehmen und
nachverfolgen“ gestartet und bewusst abgebrochen, zum Beispiel durch Beenden der
Claude-Sitzung. Der verantwortliche Kollege prüft zum vereinbarten Zeitpunkt,
erkennt die ausbleibende Rückmeldung, dokumentiert den Lauf als abgebrochen und
startet einen Ersatzlauf, der auf den bisherigen Eintrag verweist.

## Beobachtungen

Während der Erprobung festhalten, mit Datum:

| Zeitpunkt | Szenario | Frage | Antwort der unbeteiligten Person oder Beobachtung | Stimmt mit dem tatsächlichen Stand überein? |
|---|---|---|---|---|
| [Datum] | A | 1 | [...] | Ja / Nein, weil [...] |

Zusätzlich: Stellen, an denen Statusblock oder Review-Eintrag vergessen oder
veraltet waren, geschätzter Pflegeaufwand und Abweichungen vom Anwendungsfall.

## Auswertung und Ergebnis

UNBEKANNT: wird nach Abschluss ausgefüllt.

- Welche Fragen wurden mit Ja beantwortet, welche nicht, und warum?
- Welche Regeln des Anwendungsfalls haben sich bewährt, welche nicht?
- Welche Änderungen am Anwendungsfall oder am allgemeinen Prozess folgen daraus?

## Grenzen

- Zwei Personen und eine Aufgabe belegen nicht, dass der Prozess in größeren
  Teams oder bei vielen parallelen Aufgaben trägt.
- Ohne eingerichtete Überwachung wird die automatische Erkennung ausbleibender
  Rückmeldungen nicht erprobt, nur die manuelle Prüfung.
- Das Ergebnis gilt für den Anwendungsfall. Für den allgemeinen Prozess ist es
  ein Hinweis, aber kein vollständiger Nachweis.

## Statusentscheidung

Das Maintainer-Team entscheidet nach der Auswertung, ob der Anwendungsfall den
Status `erprobt` erhält. Voraussetzung nach der [Dokumentstruktur](../README.md)
sind dokumentierter Kontext, Zeitpunkt, Vorgehen, Ergebnis und Grenzen. Eine
bestandene Erprobung wird im Kopf des Anwendungsfalls als Erprobungsnachweis mit
Verweis auf dieses Dokument eingetragen.

## Änderungsverlauf

- 2026-09-22: Erprobung vorbereitet.
