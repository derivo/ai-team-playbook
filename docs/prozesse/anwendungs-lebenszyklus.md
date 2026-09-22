# Lebenszyklus gemeinsam genutzter Anwendungen

Deutsch (Standard) | [English](anwendungs-lebenszyklus.en.md)

- Status: Entwurf
- Pflegeverantwortung: Maintainer-Team (prüft Änderungen im Review)
- Inhaltlich geprüft: 2026-09-22 aus dem Anwendungsfall abgeleitet; keine Praxiserprobung belegt.
- Nächster Prüfanlass: vor einer Übernahme ins Team und bei praktischen Rückmeldungen
- Erprobungsnachweis: Keiner; nicht als erprobt ausgewiesen.
- Verbindlichkeit: Entscheidung des übernehmenden Teams.
- Anwendungsfälle: [App-Lifecycle im Unternehmen](../anwendungsfaelle/gedankenspiel-app-lifecycle.md)

Pflege und Formate: [Dokumentstruktur](../README.md).

## Problem

Mit KI-Agenten entstehen kleine Anwendungen schnell. Werden sie von anderen
genutzt, brauchen sie Betreuung, Datenverantwortung und irgendwann ein geordnetes
Ende. Fehlt ein geregelter Lebenszyklus, entstehen doppelte Anwendungen,
Experimente werden stillschweigend zu unverzichtbaren Arbeitsmitteln, und
niemand fühlt sich für Ausfälle oder Abschaltung zuständig.

## Zielgruppe

Teams und Organisationen, in denen Menschen – allein oder mit KI-Agenten –
Anwendungen für den gemeinsamen Einsatz bauen. Der Aufwand richtet sich nach der
Bedeutung: Ein begrenztes Experiment braucht weniger Abstimmung als eine
Anwendung, von der andere abhängen.

## Rollen

- **Fachlich Verantwortliche:** verantworten Nutzen und fachliche Entscheidungen.
- **Technische Betreuung mit Vertretung:** betreut Technik, Updates und Störungen.
- **Ansprechperson für neue Ideen:** ordnet Ideen zusammen mit den fachlich
  Verantwortlichen ein.
- **Betroffene Teams und Fachstellen** (etwa Betrieb, IT-Sicherheit oder
  Datenschutz): werden einbezogen, wenn Daten, Zugriffe, Betrieb oder
  Abhängigkeiten es erfordern.
- **KI-Agenten** können Arbeiten ausführen, übernehmen aber keine organisatorische
  Verantwortung.

## Ablauf

### 1. Idee sichtbar machen

Vor einer Umsetzung für den gemeinsamen Einsatz einen Eintrag im zentralen
Anwendungsverzeichnis anlegen. Der Eintrag bleibt über den gesamten Lebenszyklus
bestehen; Entwicklungsaufgaben und Änderungen werden damit verknüpft. Er
beantwortet:

- Welches Problem soll gelöst werden, und für wen?
- Gibt es bereits eine Anwendung oder eine passende Erweiterungsmöglichkeit?
- Wer übernimmt die fachliche Verantwortung?
- Welche Daten, Schnittstellen und Teams sind betroffen?
- Woran ist erkennbar, dass sich die Anwendung lohnt?

### 2. Einordnen

Die Ansprechperson prüft die Idee mit den fachlich Verantwortlichen und bezieht
Betroffene ein. Ergebnis: vorhandene Lösung nutzen, vorhandene Lösung erweitern,
begrenzten Versuch starten oder Idee zurückstellen. Entscheidung und Grund werden
im Eintrag festgehalten.

### 3. Begrenzten Versuch durchführen

Ein Versuch hat Verantwortliche, einen kleinen Nutzerkreis und einen Termin für
die Entscheidung über Fortführung oder Ende. Er ist als Experiment gekennzeichnet.
Ein persönlicher Versuch mit Testdaten kann vereinfacht starten. Sobald andere ihn
regelmäßig nutzen sollen, echte Daten angebunden werden oder ein Arbeitsablauf
davon abhängt, ist die Einordnung aus Schritt 2 erforderlich.

Abschluss: einstellen, mit neuem Ziel und Termin weiter testen oder für den
regulären Betrieb vorbereiten.

### 4. Betrieb ausdrücklich übernehmen

Vor regelmäßiger Nutzung sind die Fragen der Übernahme-Checkliste beantwortet.
Fachlich Verantwortliche und technische Betreuung bestätigen die Übernahme. Ohne
benannte Betreuung bleibt die Anwendung ein begrenzter Versuch.

### 5. Regelmäßig über Fortführung entscheiden

Zum Prüftermin werden Nutzung, Nutzen, Kosten, offene Probleme und
Betreuungsaufwand betrachtet. Entscheidung: weiterbetreiben, verbessern, mit einer
anderen Lösung zusammenführen oder abschalten. Verantwortliche und nächster
Prüftermin werden aktualisiert. Verlässt eine betreuende Person das Team, wird die
Übergabe ausdrücklich organisiert.

### 6. Geordnet abschalten

Nutzer und abhängige Teams erhalten einen Abschalttermin und gegebenenfalls eine
Alternative. Benötigte Daten werden übertragen oder exportiert, verbleibende
Daten nach den geltenden Vorgaben aufbewahrt oder gelöscht. Danach werden Jobs,
Integrationen, Zugänge, Betrieb und kostenpflichtige Dienste beendet und
Quellen und Dokumentation archiviert. Der Verzeichniseintrag bleibt mit
Abschaltdatum und Nachfolgelösung erhalten.

## Vorlagen

### Übernahme-Checkliste

| Thema | Erforderliche Antwort |
|---|---|
| Verantwortung | Wer verantwortet Nutzen und fachliche Entscheidungen? |
| Betreuung | Wer betreut Technik, Updates und Störungen; wer vertritt diese Person? |
| Ablage | Wo liegen Quellen, Dokumentation und Verzeichniseintrag? |
| Betrieb | Wo läuft die Anwendung, wer trägt Kosten und verwaltet Zugänge? |
| Daten | Welche Daten werden verarbeitet, wer erhält Zugriff, wie werden sie aufbewahrt oder gelöscht? |
| Ausfall | Wie wird ein Ausfall bemerkt, wer reagiert, wie wird währenddessen weitergearbeitet? |
| Wiederherstellung | Falls Daten oder Zustand erhalten werden müssen: Wie werden sie gesichert und wiederhergestellt? |
| Nutzung | Wer nutzt die Anwendung, und wohin werden Probleme gemeldet? |
| Ende | Wann wird der Nutzen erneut geprüft, und wie kann die Anwendung abgelöst werden? |

### Verzeichniseintrag

```text
Name und Zweck:
Status: Idee / Experiment / In Vorbereitung / In Betrieb / Wird abgelöst / Stillgelegt
Fachlich verantwortlich:
Technische Betreuung und Vertretung:
Nutzerkreis:
Quellen und Dokumentation:
Daten und Abhängigkeiten:
Betriebsort und laufende Kosten:
Nächste Entscheidung, zuständige Person und Termin:
```

## Grenzen

- Der Prozess ersetzt keine rechtlichen, Sicherheits- oder Datenschutzvorgaben;
  er sorgt nur dafür, dass die zuständigen Stellen rechtzeitig einbezogen werden.
- Anpassungspunkte: Ort des Anwendungsverzeichnisses, Schwelle für die
  Einordnung, Prüfrhythmus (etwa vierteljährlich als Startwert) und die
  beteiligten Fachstellen.
- Erfolgskriterium für eine Erprobung: Für jede erfasste Anwendung lässt sich ohne
  Nachfragen feststellen, warum sie existiert, wer sie betreut, welchen Status sie
  hat und wann die nächste Entscheidung ansteht.

## Quellen

- Abgeleitet aus dem Anwendungsfall
  [App-Lifecycle im Unternehmen](../anwendungsfaelle/gedankenspiel-app-lifecycle.md).
- Vorschlag ohne belegte Praxiserprobung.

## Änderungsverlauf

- 2026-09-22: Als allgemeiner Prozess aus dem Anwendungsfall abgeleitet.
