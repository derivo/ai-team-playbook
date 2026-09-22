# Teamprozess: Issues, Pull Requests und KI-Reviews

Deutsch (Standard) | [English](teamprozess-mensch-ki-github.en.md)

- Status: Entwurf
- Pflegeverantwortung: UNBEKANNT: noch nicht zugewiesen
- Inhaltlich geprüft: Ausgangsentwurf übernommen; keine Praxiserprobung belegt.
- Nächster Prüfanlass: vor einer Übernahme ins Team und bei praktischen Rückmeldungen
- Verbindlichkeit: Das übernehmende Team entscheidet; die folgenden Vorgaben sind ein Vorschlag.
- Beispiele: Illustrativ und fiktiv; keine dokumentierten Erfahrungsfälle.

Pflege und Formate: [Dokumentstruktur](../README.md).

Aktualisierter Prozessvorschlag zur Abstimmung im Team.

## Ziel und Grundregeln

Jeder im Team kann erkennen, wer woran arbeitet, ob ein Pull Request (PR) existiert und wer als Nächstes handeln muss. Claude Code läuft weiterhin lokal auf den Rechnern der Kollegen. GitHub ist die gemeinsame Arbeitsübersicht.

- Jede Aufgabe hat einen verantwortlichen Menschen – auch wenn Claude sie umsetzt.
- Vor Arbeitsbeginn wird die Aufgabe sichtbar übernommen.
- Jede Übergabe benennt eine konkrete Person und den nächsten Schritt.
- Automatische Reviews liefern Hinweise; die menschliche Freigabe bleibt erforderlich.

## Der Ablauf

### 1. Aufgabe übernehmen

Vor dem Start von Claude ein bestehendes GitHub-Issue verwenden oder eines anlegen. Ziel und Fertig-Kriterium kurz beschreiben. Prüfen, ob bereits jemand daran arbeitet. Der zuständige Kollege trägt sich als Verantwortlicher ein und setzt den Stand auf **In Arbeit**. Ohne vorhandenen PR steht ausdrücklich **Noch kein PR** im Issue.

### 2. Claude beauftragen

Der Kollege gibt Claude das Issue, das Ziel und die Grenzen des Auftrags mit. Claude prüft vorhandene verknüpfte PRs, damit keine doppelte Umsetzung entsteht. Unklare Anforderungen klärt der verantwortliche Kollege.

### 3. Arbeit früh sichtbar machen

Sobald erste Änderungen vorliegen, erstellt Claude einen **Draft-PR** und verknüpft ihn mit dem Issue. Der Draft zeigt laufende Arbeit; er ist noch keine Aufforderung zum Review.

### 4. Status aktuell halten

Bei Beginn, Pause, Blockade und Übergabe den Statusblock im Issue aktualisieren. Claude soll das übernehmen; der verantwortliche Kollege kontrolliert es spätestens beim Unterbrechen seiner Arbeit.

Bei einer Blockade festhalten, was fehlt und wer als Nächstes handeln muss. Datum und Uhrzeit der Aktualisierung mitführen: Ein alter Eintrag „In Arbeit“ beweist nicht, dass der Agent noch läuft.

### 5. Review übergeben

Nach den vereinbarten Prüfungen kontrolliert der verantwortliche Kollege Ergebnis und Prüfnachweise. Er markiert den PR als reviewbereit und fragt einen konkreten Kollegen als Reviewer an. Im Issue steht **Wartet auf Review**, einschließlich Reviewer und nächstem Schritt.

Jeder KI-Review wird vor dem Start am PR sichtbar übernommen und nach dem unten beschriebenen Review-Ablauf begleitet. Im Issue wird auf diesen Review-Eintrag verwiesen.

Automatische Review-Hinweise werden geprüft und bearbeitet oder begründet verworfen. Bei Änderungswünschen geht der nächste Schritt zurück an den Autor. Dieser beauftragt Claude mit der Überarbeitung, lässt erneut prüfen und fordert anschließend ein neues Review an.

### 6. Abschließen

Nach menschlicher Freigabe und erfüllten Projektprüfungen gemäß Teamregeln mergen. Bevor das ursprüngliche Issue geschlossen wird, werden alle konkret erkannten, noch offenen Nacharbeiten als eigene GitHub-Issues angelegt.

- Jedes Nacharbeits-Issue beschreibt den offenen Punkt, den relevanten Kontext und den Grund für die Nacharbeit. Zugehörige Review-Kommentare oder Entscheidungen werden verlinkt.
- Im ursprünglichen Issue werden sämtliche Nacharbeits-Issues verlinkt. Jedes Nacharbeits-Issue verweist zurück auf das ursprüngliche Issue und den zugehörigen PR. So bleibt die gesamte Entscheidungskette nachvollziehbar.
- Erst wenn die offenen Nacharbeiten erfasst und verlinkt sind, wird das ursprüngliche Issue geschlossen. Das bedeutet nicht, dass die Nacharbeiten bereits erledigt sind.
- Reviewende können eine erfasste Nacharbeit als nicht erforderlich einstufen. Dann wird das Nacharbeits-Issue mit einer kurzen Begründung geschlossen. Es wird nicht gelöscht; Kontext und Entscheidung bleiben erhalten.

Erkannte Nacharbeiten werden somit nicht nur in Kommentaren, Chats oder lokalen Agent-Sitzungen festgehalten. Sie sind als verknüpfte Issues sichtbar, bis sie umgesetzt oder ausdrücklich verworfen wurden.

## KI-Reviews sichtbar übernehmen und nachverfolgen

Der Aufgabenstand bleibt im Issue. Der konkrete Code-Review wird am PR dokumentiert, weil er sich auf einen bestimmten Commit bezieht. Ein Link im Issue führt zum aktuellen Review-Eintrag. So werden Detailangaben nicht an zwei Stellen parallel gepflegt.

### Vor dem Start

Der ausführende Kollege oder die Automation prüft, ob bereits ein Review für diesen PR und Commit übernommen wurde. Vor dem Start wird ein Review-Eintrag mit verantwortlichem Menschen, Agent/Sitzung, geprüftem Commit und Startzeit angelegt. Auch der Zeitpunkt der nächsten erwarteten Rückmeldung wird festgehalten.

Ein vorhandener oder unklarer Lauf wird zuerst mit seinem Verantwortlichen geklärt. Ein weiterer unabhängiger Review wird nur bewusst als solcher gestartet und kenntlich gemacht.

### Während des Reviews

Der Agent oder seine begleitende Automation aktualisiert den Review-Eintrag regelmäßig mit letzter Rückmeldung und kurzem Zwischenstand. Als zunächst zu erprobender Richtwert gelten zehn Minuten zwischen Rückmeldungen.

Bleibt die vereinbarte Rückmeldung aus, prüft eine vom Review-Agent unabhängige Überwachung den Lauf, markiert ihn als **Zustand prüfen** und benachrichtigt den verantwortlichen Kollegen. Ein abgestürzter Agent kann seinen eigenen Ausfall nicht zuverlässig melden. Solange diese Überwachung nicht eingerichtet ist, übernimmt der benannte Kollege die Prüfung zum vereinbarten Zeitpunkt; eine automatische Benachrichtigung gibt es dann nicht.

### Bei Blockade oder Abbruch

Eine bekannte Blockade wird mit Ursache und nächstem Schritt dokumentiert. Eine überfällige Rückmeldung bedeutet dagegen nur, dass der Zustand unklar ist, nicht automatisch einen Abbruch.

Vor einer Wiederaufnahme oder einem Ersatzlauf wird geklärt, ob der bisherige Lauf noch arbeitet. Bereits geprüfte Bereiche, Befunde und offene Prüfpunkte bleiben im bisherigen Eintrag erhalten. Der neue Lauf verweist darauf und übernimmt den verfügbaren Zwischenstand. Ein abgebrochener Lauf wird ausdrücklich als abgebrochen dokumentiert; er gilt nicht als abgeschlossener Review.

### Beim Abschluss

Das veröffentlichte Review-Ergebnis wird verlinkt. Der Eintrag nennt den tatsächlich geprüften Commit und ob der Review vollständig war. Neue Commits sind nicht automatisch durch einen älteren Review abgedeckt; der zuständige Reviewer entscheidet, welche erneute Prüfung erforderlich ist. Die menschliche Freigabe bleibt erforderlich.

### Optionale Labels zum Filtern

Der Review-Eintrag ist verbindlich. Wenn das Team zusätzlich nach dem Review-Zustand filtern möchte, verwendet es am PR dieses kleine Label-Set. Es gilt für einen einzelnen maßgeblichen KI-Review-Lauf; vorherige Zustandslabels werden beim Wechsel entfernt.

| Label | Bedeutung |
|---|---|
| `review:ki-laeuft` | Review übernommen und als laufend gemeldet |
| `review:ki-blockiert` | Bekannte Blockade gemeldet |
| `review:ki-pruefen` | Rückmeldung überfällig oder Laufzustand unklar |
| `review:ki-abgebrochen` | Lauf beendet, Review unvollständig; Zwischenstand dokumentiert |
| `review:ki-fertig` | Vollständiges Ergebnis für den angegebenen Commit veröffentlicht |

Labels allein verhindern keine gleichzeitigen Starts. Wenn mehrere Automationen Reviews starten, muss eine zentrale Vergabe technisch sicherstellen, dass pro PR und Commit nur ein regulärer Lauf die Aufgabe übernimmt. Bis dahin stimmen sich die verantwortlichen Kollegen vor dem Start ab.

### Vorlage für den Review-Eintrag am PR

```text
Verantwortlicher Kollege: Ben
Agent/Sitzung: [eindeutige Bezeichnung des Review-Laufs]
Geprüfter Commit: [Commit-ID]
Review-Stand: Läuft / Blockiert / Zustand prüfen / Abgebrochen / Fertig
Gestartet: [Datum und Uhrzeit]
Letzte Rückmeldung: [Datum und Uhrzeit]
Nächste Rückmeldung erwartet bis: [Datum und Uhrzeit]
Zwischenstand: [geprüfte Bereiche, bisherige Befunde, offene Prüfpunkte]
Nächster Schritt und zuständige Person: [...]
Ergebnis oder vorheriger Lauf: [Link, soweit vorhanden]
```

## Gemeinsame Statusangaben

| Stand | Bedeutung |
|---|---|
| Offen | Noch nicht übernommen |
| In Arbeit | Ein Kollege bearbeitet die Aufgabe, gegebenenfalls mit Claude |
| Pausiert | Arbeit bewusst unterbrochen |
| Blockiert | Eine konkrete Voraussetzung oder Entscheidung fehlt |
| Wartet auf Review | Ein benannter Reviewer ist als Nächstes dran |
| In Überarbeitung | Der Autor bearbeitet Review-Rückmeldungen |
| Erledigt | Änderungen gemergt und Issue abgeschlossen |

## Statusvorlage für die Issue-Beschreibung

Diesen Block aktuell halten, damit niemand den Kommentarverlauf durchsuchen muss. „Verantwortlich“ bezeichnet den Besitzer der Aufgabe. „Nächster Schritt“ benennt die Person, die jetzt handeln muss.

```text
Verantwortlich: Anna
Agent: Annas lokaler Claude Code
Stand: Wartet auf Review
PR: [Link oder „Noch kein PR“]
KI-Review: [Link zum aktuellen Review-Eintrag oder „Noch nicht gestartet“]
Nächster Schritt: Ben prüft die Änderungen.
Blockade: Keine
Zuletzt aktualisiert: [Datum und Uhrzeit]
```

## Einführung

Zunächst mit zwei Kollegen an einer Aufgabe ausprobieren. Erfolgskriterium: Ein unbeteiligter Kollege erkennt anhand des Issues ohne Nachfragen den Verantwortlichen, den zugehörigen PR, den Arbeitsstand und die nächste zuständige Person.

Für den ersten Versuch können Statuspflege und Übernahme manuell erfolgen. Zusätzlich einen unterbrochenen KI-Review erproben: Der verantwortliche Kollege muss den fehlenden Fortschritt erkennen und den bisherigen Stand vor einem Ersatzlauf nachvollziehen können.

Automatische Rückmeldungen, Überwachung und Benachrichtigungen müssen gesondert eingerichtet werden. Die oben beschriebenen Labels und Vorlagen allein stellen diese Funktionen nicht bereit.
