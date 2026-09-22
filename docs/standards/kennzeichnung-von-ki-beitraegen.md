# Standard: Kennzeichnung von KI-Beiträgen

Deutsch (Standard) | [English](kennzeichnung-von-ki-beitraegen.en.md)

- Status: Entwurf
- Pflegeverantwortung: Maintainer-Team (prüft Änderungen im Review)
- Inhaltlich geprüft: 2026-09-22 gegen die Commit-Praxis dieses Repositorys; keine Praxiserprobung belegt.
- Nächster Prüfanlass: vor einer Übernahme ins Team und bei praktischen Rückmeldungen
- Erprobungsnachweis: Keiner; nicht als erprobt ausgewiesen.
- Verbindlichkeit: Entscheidung des übernehmenden Teams.
- Anwendungsfälle: Noch keine.

Pflege und Formate: [Dokumentstruktur](../README.md).

## Problem

Ohne Kennzeichnung ist später nicht erkennbar, welche Änderungen, Texte oder
Reviews mit KI-Unterstützung entstanden sind. Das erschwert Reviews, die
Einschätzung von Fehlerquellen und die Nachvollziehbarkeit von Entscheidungen.

## Zielgruppe

Teams, die KI-Agenten an Code, Dokumentation, Reviews oder Kommunikation
mitarbeiten lassen.

## Rollen

- **Verantwortlicher Mensch:** bleibt Urheber im Sinne der Verantwortung und
  sorgt für die Kennzeichnung.
- **KI-Agent:** setzt die vereinbarte Kennzeichnung, wenn er Commits,
  Beschreibungen oder Kommentare erstellt.
- **Team:** legt fest, was gekennzeichnet wird und in welcher Form.

## Ablauf

### 1. Kennzeichnungspflichtige Beiträge festlegen

Das Team legt fest, welche Beiträge gekennzeichnet werden, zum Beispiel:

- Commits, an denen ein Agent wesentlich mitgearbeitet hat,
- Beschreibungen von Änderungsvorschlägen,
- automatische oder KI-gestützte Review-Kommentare,
- veröffentlichte Dokumente mit wesentlichem KI-Anteil.

### 2. Einheitliche Form verwenden

- **Commits:** ein Trailer am Ende der Commit-Nachricht, zum Beispiel
  `Co-Authored-By: [Agent und Modell] <[Adresse]>`.
- **Änderungsvorschläge:** ein Hinweis am Ende der Beschreibung.
- **Reviews:** der Review-Eintrag nennt Agent und Sitzung.

### 3. Verantwortung nicht übertragen

Die Kennzeichnung beschreibt die Mitwirkung. Verantwortung, Freigabe und
Urheberschaft im Sinne des Projekts bleiben beim Menschen, der den Beitrag
einbringt.

## Vorlagen

```text
Co-Authored-By: [Agent und Modell] <[Adresse]>
```

## Grenzen

- Die Kennzeichnung sagt nichts über die Qualität eines Beitrags.
- Rechtliche Fragen zu Urheberrecht und Lizenzierung KI-generierter Inhalte
  regelt dieser Standard nicht.
- Anpassungspunkte: Umfang der Kennzeichnung, genaue Form, Schwelle für
  „wesentliche“ Mitarbeit.

## Quellen

- Abgeleitet aus der Commit-Praxis dieses Repositorys, dessen Commits einen
  `Co-Authored-By`-Trailer für den mitarbeitenden Agenten tragen.
- Vorschlag ohne belegte Praxiserprobung.

## Änderungsverlauf

- 2026-09-22: Als Standard angelegt.
