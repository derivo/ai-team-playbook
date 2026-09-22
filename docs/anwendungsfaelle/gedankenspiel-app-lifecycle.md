# Gedankenspiel: Von der App-Idee bis zur Abschaltung

Deutsch (Standard) | [English](gedankenspiel-app-lifecycle.en.md)

- Status: Entwurf
- Pflegeverantwortung: Maintainer-Team (prüft Änderungen im Review)
- Inhaltlich geprüft: Ausgangsentwurf übernommen; keine Praxiserprobung belegt.
- Nächster Prüfanlass: vor einer Übernahme ins Team und bei praktischen Rückmeldungen
- Erprobungsnachweis: Keiner; nicht als erprobt ausgewiesen.
- Verbindlichkeit: Das übernehmende Team entscheidet; die folgenden Vorgaben sind ein Vorschlag.
- Beispiele: Illustrativ und fiktiv; keine dokumentierten Erfahrungsfälle.
- Allgemeiner Prozess: [Lebenszyklus gemeinsam genutzter Anwendungen](../prozesse/anwendungs-lebenszyklus.md); dieser Anwendungsfall ist eine konkrete Ausprägung davon.

Pflege und Formate: [Dokumentstruktur](../README.md).

Diskussionsvorschlag für das Team, noch keine beschlossene Unternehmensregel.

## Ausgangspunkt

Eine schnell entwickelte Anwendung braucht auch nach ihrer ersten Nutzung Betreuung. Deshalb soll jede gemeinsam genutzte App einen Zweck, einen Verantwortlichen und einen geregelten Lebenszyklus haben. Der Aufwand dafür richtet sich nach ihrer Bedeutung: Ein begrenztes Experiment braucht weniger Abstimmung als eine Anwendung, von der andere Teams abhängig sind.

## 1. Idee sichtbar machen

Vor einer Umsetzung für den gemeinsamen Einsatz wird eine kurze Ideenkarte in einem zentralen Anwendungsverzeichnis angelegt. Zum Einstieg kann das eine gemeinsame GitHub-Projects-Übersicht mit einem Issue pro Anwendung sein. Das Anwendungs-Issue bleibt über den Lebenszyklus bestehen; einzelne Entwicklungsaufgaben und PRs werden damit verknüpft.

Die Ideenkarte beantwortet:

- Welches Problem soll gelöst werden, und für wen?
- Gibt es dafür bereits eine Anwendung oder eine passende Erweiterungsmöglichkeit?
- Wer übernimmt die fachliche Verantwortung?
- Welche Daten, Schnittstellen und Teams sind betroffen?
- Woran erkennen wir, dass sich die Anwendung lohnt?

## 2. Kurz abstimmen und einordnen

Eine benannte Ansprechperson im Team prüft die Idee zusammen mit dem fachlich Verantwortlichen. Betroffene Teams werden einbezogen; IT, Betrieb oder Datenschutz kommen hinzu, wenn Daten, Zugriffe, Hosting oder Abhängigkeiten dies erfordern.

Ergebnis: vorhandene Lösung nutzen, vorhandene Lösung erweitern, begrenzten Versuch starten oder Idee zurückstellen. Nicht jede Idee benötigt eine große Freigaberunde, aber die Entscheidung und ihr Grund werden festgehalten.

## 3. Einen begrenzten Versuch erlauben

Ein Experiment erhält einen Verantwortlichen, einen kleinen Nutzerkreis und einen Termin zur Entscheidung über Fortführung oder Ende. Es wird als Experiment gekennzeichnet und nicht stillschweigend zum dauerhaften Arbeitsmittel.

Ein persönlicher Versuch mit Testdaten kann vereinfacht starten. Sobald andere Menschen ihn regelmäßig nutzen sollen, echte Unternehmensdaten angebunden werden oder ein Arbeitsablauf davon abhängt, ist die Abstimmung aus Schritt 2 erforderlich.

Am Ende des Versuchs wird entschieden: einstellen, mit neuem Ziel und Termin weiter testen oder für den regulären Betrieb vorbereiten.

## 4. Den Betrieb ausdrücklich übernehmen

Vor regelmäßiger Nutzung müssen mindestens folgende Fragen beantwortet sein:

| Thema | Erforderliche Antwort |
|---|---|
| Verantwortung | Wer verantwortet Nutzen und fachliche Entscheidungen? |
| Betreuung | Wer betreut Technik, Updates und Störungen; wer vertritt diese Person? |
| Ablage | Wo liegen Repository, Dokumentation und Eintrag im Anwendungsverzeichnis? |
| Betrieb | Wo läuft die App, wer trägt Kosten und verwaltet Zugänge? |
| Daten | Welche Daten werden verarbeitet, wer erhält Zugriff und wie werden sie aufbewahrt oder gelöscht? |
| Ausfall | Wie wird ein Ausfall bemerkt, wer reagiert und wie arbeitet das Team währenddessen weiter? |
| Wiederherstellung | Falls Daten oder Zustand erhalten werden müssen: Wie werden sie gesichert und wiederhergestellt? |
| Nutzung | Wer sind die Nutzer, und wohin melden sie Probleme? |
| Ende | Wann wird der Nutzen erneut geprüft, und wie kann die App abgelöst werden? |

Der fachlich Verantwortliche und die technische Betreuung bestätigen die Übernahme. Ohne benannte Betreuung bleibt die Anwendung ein begrenzter Versuch. Ein KI-Agent kann Arbeiten ausführen, übernimmt aber keine organisatorische Verantwortung.

## 5. Regelmäßig über Fortführung entscheiden

Zum festgelegten Prüftermin werden Nutzung, Nutzen, Kosten, offene Probleme und Betreuungsaufwand betrachtet. Als Startvorschlag bietet sich eine vierteljährliche Prüfung an; das Team passt den Rhythmus an die Anwendung an.

Die Entscheidung lautet: weiterbetreiben, verbessern, mit einer anderen Lösung zusammenführen oder abschalten. Verantwortliche und nächster Prüftermin werden aktualisiert. Verlässt der Betreuer das Team, wird die Übergabe ausdrücklich organisiert.

## 6. Geordnet abschalten

Nutzer und abhängige Teams erhalten einen Abschalttermin und gegebenenfalls eine Alternative. Benötigte Daten werden übertragen oder exportiert; verbleibende Daten werden nach den geltenden Vorgaben aufbewahrt oder gelöscht. Danach werden Jobs, Integrationen, Zugänge, Hosting und kostenpflichtige Dienste beendet. Repository und Dokumentation werden passend archiviert.

Der Verzeichniseintrag bleibt mit Abschaltdatum und Nachfolgelösung erhalten, damit später niemand dieselbe Anwendung unbemerkt neu aufbaut.

## Minimaler Eintrag pro Anwendung

```text
Name und Zweck:
Status: Idee / Experiment / In Vorbereitung / In Betrieb / Wird abgelöst / Stillgelegt
Fachlich verantwortlich:
Technische Betreuung und Vertretung:
Nutzerkreis:
Repository und Dokumentation:
Daten und Abhängigkeiten:
Betriebsort und laufende Kosten:
Nächste Entscheidung, zuständige Person und Termin:
```

## Konkretes Beispiel

Eine Kollegin möchte eine kleine App zur Aufbereitung von Kundenlisten bauen. Sie erfasst die Idee, prüft vorhandene Lösungen und stimmt die geplante Datennutzung mit den zuständigen Personen ab. Ein zeitlich begrenzter Versuch startet mit Testdaten.

Nach dem Versuch zeigt sich ausreichender Nutzen. Bevor weitere Kollegen die App regelmäßig verwenden, werden Betreuung, Zugriffe, Betrieb und Umgang mit Ausfällen geklärt. Bei einer späteren Prüfung übernimmt ein vorhandenes System die Funktion. Die Daten werden übertragen und die App wird geordnet abgeschaltet.

## Einstieg im Unternehmen

Den Vorschlag an einer neuen Idee und einer bereits genutzten kleinen App erproben. Dafür zuerst den gemeinsamen Ablageort und die Ansprechperson für neue Ideen festlegen.

Erfolgskriterium: Für beide Anwendungen lässt sich ohne Nachfragen feststellen, warum sie existieren, wer sie betreut, welchen Status sie haben und wann die nächste Entscheidung ansteht.
