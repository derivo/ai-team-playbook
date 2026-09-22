# Dokumentstruktur und Pflege

[English version](README.en.md)

## Zweck und Zielgruppe

Diese Bibliothek bietet Teams und KI-Agenten anpassbare Standards, Prozesse und
Workflows. Leser sollen einen passenden Entwurf finden, seine Grenzen erkennen
und eine bewusste Anpassung für ihren Kontext dokumentieren können.

## Umfang und Quellen

Enthalten sind Dokumente, Vorlagen und Skills zur Inhaltspflege. Nicht enthalten
sind installierte Automationen, ein verbindliches Firmenhandbuch oder eine
festgelegte Lizenz. Quellen sind der konkrete Änderungsauftrag, die betroffenen
Dokumente und tatsächlich geprüfte Nachweise. Erfahrungen werden nicht erfunden.

## Ablage und Formate

- [Projektübersicht](../README.md): Zweck, Einstieg, Status und Arbeitsstand.
- [Vision und Wiederaufnahme](../vision.md): Zielbild, aktueller Stand und nächste Schritte.
- [Projektregeln](../AGENTS.md): Regeln für die Arbeit am Repository.
- `entwuerfe/`: die beiden übernommenen Ausgangsdokumente, getrennt voneinander.
- [Inhaltsvorlage](vorlagen/inhalt.md): Struktur für neue oder angepasste Inhalte.
- [Änderungsanfrage](vorlagen/aenderungsanfrage.md): lokal nutzbar, später als Issue.
- [Pull-Request-Vorlage](vorlagen/pull-request.md): lokaler PR-Entwurf, später als PR.
- `.agents/skills/` im Projekt: Skills für Inhalte, Überarbeitungen und Anfragen/PRs.

Dokumente verwenden UTF-8-Markdown (`.md`), deutsche Prosa, eine H1-Überschrift
und logisch folgende H2/H3-Abschnitte. Dateinamen sind sprechend, kleingeschrieben
und mit Bindestrichen getrennt. Links sind relativ; externe URLs nur nach Prüfung.
Codeblöcke nennen ihre Sprache, bei Formulartext `text`. Tabellen dienen echten
Vergleichen. Keine neue Tool-Abhängigkeit nur für die Dokumentpflege einführen.

Jeder öffentliche Inhalt besteht aus einem Sprachpaar. Die deutsche
Standardfassung verwendet den Dateinamen ohne Sprachsuffix, zum Beispiel
`vision.md`. Die englische Fassung verwendet `.en.md`, zum Beispiel
`vision.en.md`. Beide Fassungen stehen im selben Verzeichnis, verlinken einander
am Anfang und enthalten denselben fachlichen Stand. Eine Inhaltsänderung ist erst
vollständig, wenn beide Fassungen aktualisiert und geprüft sind.

Neue Inhalte folgen: **Problem → Zielgruppe → Rollen → Ablauf → Vorlagen →
Grenzen**. Pflegeangaben stehen davor, Quellen und Änderungsverlauf danach.
Die übernommenen Erstentwürfe behalten ausdrücklich ihre eigene Gliederung und
ihren Originaltext; ihre Einordnung und Pflegeangaben sind ergänzt. Eine spätere
Umgliederung benötigt einen konkreten Auftrag.

## Status und Verbindlichkeit

| Status | Voraussetzung |
| --- | --- |
| Entwurf | Vorschlag; keine belegte Erprobung behauptet |
| erprobt | Dokumentierter Kontext, Zeitpunkt, Vorgehen, Ergebnis und Grenzen der Erprobung |
| abgelöst | Datum, Grund und Verweis auf Nachfolger oder ausdrücklicher Hinweis, dass keiner existiert |

Diese Statuswerte betreffen die Reife eines Dokuments, nicht den Arbeitsstand
eines Issues oder den Betriebsstatus einer App. Bei inhaltlichen Änderungen an
einem erprobten Dokument prüfen, ob der Nachweis noch gilt; sonst auf Entwurf
zurücksetzen. Eine Ablösung erhält die bisherige Entscheidung nachvollziehbar.

Jedes Team entscheidet selbst, welche Teile es übernimmt und verbindlich macht.
„Muss“ in einem Prozessentwurf gilt innerhalb des vorgeschlagenen Prozesses;
es verpflichtet durch die Aufnahme in diese Bibliothek noch kein Team.

## Zuständigkeit und Aktualisierungsprüfung

Jeder Inhalt nennt Status, Pflegeverantwortung, letzten inhaltlichen Prüfstand,
nächsten Prüfanlass und Erprobungsnachweis. Nicht zugewiesene Verantwortung heißt
`UNBEKANNT: Pflegeverantwortung`; keine Person eigenmächtig eintragen.
Die Pflegeverantwortlichen prüfen bei Quellenänderungen, praktischen Rückmeldungen
und vor einer Übernahme ins Team, ob Aussagen und Nachweise weiter gelten. Das
übernehmende Team benennt Zuständige und einen passenden nächsten Prüftermin.
Ein Agent kann die Prüfung unterstützen; er ersetzt keine menschliche Entscheidung.

## Änderungen und Anfragen

Vor einer Änderung bestehende Dokumente und offene Anfragen prüfen. Lokal eine
Kopie der Anfragevorlage mit eindeutigem Dateinamen und relativen Links verwenden.
Die Anfrage hält Problem, Ziel, Umfang, Akzeptanzkriterien und Entscheidung fest.
Umgesetzte Änderungen bekommen einen kurzen Eintrag im Änderungsverlauf; Details
stehen in der verlinkten Anfrage statt in mehreren parallelen Protokollen.

Sobald GitHub eingerichtet ist, werden Anfragen als Issues und Änderungen als
verknüpfte PRs nachvollziehbar. Bestehende lokale Anfragen weiterverwenden und auf
das überführte Issue verweisen. Keine erfundenen Issue-Nummern, PRs oder URLs.
Ein PR-Entwurf allein erteilt keine Erlaubnis für Commit, Push oder Veröffentlichung.
Konkrete Nacharbeiten als eigene Anfragen erfassen und gegenseitig verlinken;
Ablehnungen mit Grund erhalten. Bei Anwendung des Teamprozesses gelten dessen
präzisere Regeln für Nacharbeits-Issues.

## Prüfmaßstab

Vor Abschluss: Markdown und Skill-Metadaten mechanisch prüfen, relative Links
auflösen, Aussagen gegen den Auftrag und Quellen abgleichen und Änderungen auf
Secrets/echte Personendaten prüfen. Beispiele sind ausdrücklich fiktiv.
Diagramme benötigen einen Render-Check, falls welche hinzugefügt werden.
Vorhandene Formatter nur auf geänderte Dateien anwenden. Fehlende Werkzeuge und
die Grenzen von Ersatzprüfungen offen nennen; kein unbelegtes „alles geprüft“.

Fertig ist eine Änderung mit beobachtetem Prüfergebnis, erfüllten
Akzeptanzkriterien und benannten offenen Punkten. Status „Entwurf“ kann trotz
bestandener Dokumentprüfung bestehen bleiben: Sie belegt keine Praxiserprobung.
