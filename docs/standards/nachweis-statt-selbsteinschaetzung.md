# Standard: Nachweis statt Selbsteinschätzung

Deutsch (Standard) | [English](nachweis-statt-selbsteinschaetzung.en.md)

- Status: Entwurf
- Pflegeverantwortung: Maintainer-Team (prüft Änderungen im Review)
- Inhaltlich geprüft: 2026-09-22 gegen die Projektregeln und die Dokumentstruktur dieses Repositorys; keine Praxiserprobung belegt.
- Nächster Prüfanlass: vor einer Übernahme ins Team und bei praktischen Rückmeldungen
- Erprobungsnachweis: Keiner; nicht als erprobt ausgewiesen.
- Verbindlichkeit: Entscheidung des übernehmenden Teams.
- Anwendungsfälle: Noch keine.

Pflege und Formate: [Dokumentstruktur](../README.md).

## Problem

KI-Agenten formulieren Ergebnisse überzeugend, auch wenn sie nicht geprüft oder
unvollständig sind. Fehlende Informationen werden leicht plausibel aufgefüllt,
Quellen oder Testergebnisse erfunden. Wer sich auf solche Aussagen verlässt,
übernimmt Fehler ungeprüft.

## Zielgruppe

Alle, die Ergebnisse von KI-Agenten beauftragen, prüfen oder weitergeben – bei
Code, Dokumentation, Analysen oder Recherchen.

## Rollen

- **KI-Agent:** belegt Aussagen durch Beobachtungen und kennzeichnet Unbekanntes.
- **Verantwortlicher Mensch:** prüft die Nachweise, bevor er ein Ergebnis
  weitergibt oder freigibt.
- **Reviewer:** prüft, ob die Nachweise die Aussagen tragen.

## Ablauf

### 1. Fertig-Kriterium vorab festlegen

Vor der Arbeit wird ein prüfbares Kriterium vereinbart, zum Beispiel ein Test,
ein Befehl mit erwartetem Ergebnis oder ein beobachtbares Verhalten.

### 2. Beobachtung melden, nicht Einschätzung

Eine Fertig-Meldung nennt, was geprüft wurde und mit welchem Ergebnis: Befehl und
Ergebnis, Testname und Ausgang, beobachtete Datei oder sichtbares Verhalten.
„Sollte funktionieren“ ist kein Nachweis.

### 3. Unbekanntes kennzeichnen

Fehlende Informationen werden als `UNBEKANNT: …` markiert statt aufgefüllt.
Quellen, URLs, Zahlen und Erfahrungsbelege werden nie erfunden; eine Quelle wird
nur genannt, wenn sie in derselben Arbeitssitzung tatsächlich abgerufen wurde.

### 4. Fehler und Grenzen offen nennen

Fehlgeschlagene Prüfungen werden mit Anzahl und Ursache gemeldet. Nicht
durchgeführte Prüfungen und die Grenzen einer Ersatzprüfung werden benannt.
Eine formale Prüfung belegt keine praktische Erprobung.

## Vorlagen

```text
Ergebnis: [was erreicht wurde]
Nachweis: [Befehl/Test/Beobachtung und Ergebnis]
Nicht geprüft: [was offen blieb und warum]
UNBEKANNT: [fehlende Information, falls vorhanden]
```

## Grenzen

- Der Standard sagt nichts darüber, wie gründlich geprüft werden muss; das legt
  das Team je nach Risiko fest.
- Nachweise können selbst fehlerhaft sein; menschliche Prüfung bleibt nötig.
- Anpassungspunkte: Mindestprüfungen je Art der Änderung, Form der Fertig-Meldung.

## Quellen

- Abgeleitet aus den [Projektregeln](../../AGENTS.md) und dem Prüfmaßstab der
  [Dokumentstruktur](../README.md) dieses Repositorys.
- Vorschlag ohne belegte Praxiserprobung.

## Änderungsverlauf

- 2026-09-22: Als Standard angelegt.
