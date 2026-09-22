# Standard: Labeling AI contributions

[Deutsch (Standard)](kennzeichnung-von-ki-beitraegen.md) | English

- Status: Draft
- Maintainer: maintainer team (reviews changes)
- Content checked: 2026-09-22 against the commit practice of this repository; no practical use has been proven.
- Next review trigger: before team adoption and when practical feedback arrives
- Evidence of practical use: None; not marked as proven.
- Adoption: Decision of the adopting team.
- Use cases: None yet.

Maintenance and formats: [Documentation structure](../README.en.md).

## Problem

Without labeling, it is later impossible to tell which changes, texts, or reviews
were created with AI support. This makes reviews, the assessment of error
sources, and the traceability of decisions harder.

## Audience

Teams that let AI agents contribute to code, documentation, reviews, or
communication.

## Roles

- **Responsible person:** remains the author in terms of responsibility and
  ensures the labeling.
- **AI agent:** applies the agreed labeling when creating commits, descriptions,
  or comments.
- **Team:** defines what is labeled and in which form.

## Process

### 1. Define which contributions are labeled

The team defines which contributions are labeled, for example:

- commits to which an agent contributed substantially,
- descriptions of change proposals,
- automated or AI-assisted review comments,
- published documents with a substantial AI share.

### 2. Use a consistent form

- **Commits:** a trailer at the end of the commit message, for example
  `Co-Authored-By: [agent and model] <[address]>`.
- **Change proposals:** a note at the end of the description.
- **Reviews:** the review record names the agent and session.

### 3. Do not transfer responsibility

The label describes the contribution. Responsibility, approval, and authorship in
the project's sense remain with the person who submits the contribution.

## Templates

```text
Co-Authored-By: [agent and model] <[address]>
```

## Limits

- The label says nothing about the quality of a contribution.
- This standard does not address legal questions about copyright and licensing
  of AI-generated content.
- Adaptation points: scope of labeling, exact form, threshold for a "substantial"
  contribution.

## Sources

- Derived from the commit practice of this repository, whose commits carry a
  `Co-Authored-By` trailer for the contributing agent.
- Proposal without proven practical use.

## Change history

- 2026-09-22: Created as a standard.
