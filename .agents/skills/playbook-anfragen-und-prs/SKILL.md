---
name: playbook-anfragen-und-prs
description: Änderungsanfragen und Pull-Request-Beschreibungen für das AI Team Playbook erstellen, mit nachvollziehbaren Verknüpfungen und Prüfnachweisen; zunächst lokal nutzbar.
---

# Änderungsanfragen und Pull Requests

Deutsch (Standard) | [English](SKILL.en.md)

Lies [Dokumentstruktur und Pflege](../../../docs/README.md). Prüfe vorhandene
Anfragen und Änderungen, damit kein zweiter Vorgang zum selben Anliegen entsteht.
Verlinkte Issues oder PRs mit Beschreibung und sämtlichen Kommentarsträngen lesen,
bevor du Entscheidungen übernimmst; fehlenden Zugriff offen nennen.

## Änderungsanfrage

Verwende die [Anfragevorlage](../../../docs/vorlagen/aenderungsanfrage.md).
Formuliere Problem, gewünschten Zustand, Grenzen und beobachtbare Akzeptanzkriterien.
Halte Verantwortung, Entscheidung und nächsten Schritt fest. Verwende lokale
relative Links, solange keine echten GitHub-Vorgänge existieren. Lege eine
angefragte lokale Anfrage mit eindeutigem sprechendem Dateinamen am mit dem Nutzer
vereinbarten Ort ab; ohne Ortsvorgabe im Projekt unter `docs/`.
Erstelle öffentliche Anfragen als deutsches Standarddokument und englische
`.en.md`-Fassung; beide verlinken einander und enthalten denselben Entscheidungsstand.

## Pull Request

Verwende die [PR-Vorlage](../../../docs/vorlagen/pull-request.md). Ein Titel
benennt die konkrete Änderung und den betroffenen Inhalt. Die Beschreibung erklärt
Zweck, resultierendes Verhalten, Umfang und beobachtete Prüfnachweise. Nenne bei
öffentlichen Inhalten ausdrücklich die Prüfung beider Sprachfassungen. Passe
Titel und Beschreibung an den endgültigen Änderungsumfang an.

Verknüpfe die zugrunde liegende Anfrage. Abschlussverknüpfungen wie `Closes #…`
nur für echte, vollständig erfüllte Issues verwenden. Offene Nacharbeiten separat
und gegenseitig verlinken; Ablehnungen mit Grund dokumentieren. Bei Anwendung des
[Teamprozesses](../../../docs/anwendungsfaelle/teamprozess-mensch-ki-github.md) dessen
Review-Übernahme, Commit-Bezug und Nacharbeitsregeln berücksichtigen.

Ohne eingerichtetes Remote einen lokalen PR-Entwurf liefern. Ein echter PR
benötigt einen separaten Auftrag und vorhandene veröffentlichbare Änderungen;
vor jedem Commit explizite Freigabe einholen. Fehlen Voraussetzungen, benenne sie,
statt Remote, Commit oder Push eigenmächtig nachzuholen. Eine bloße Anfrage zum
Format erlaubt keine externe Erstellung.

Vor Ausgabe Links und Nachweise prüfen. Keine Tests als bestanden nennen, die
nicht gelaufen sind, und keine PR-URL behaupten, solange kein PR erstellt wurde.
