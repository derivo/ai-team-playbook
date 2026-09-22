# Standard: Evidence instead of self-assessment

[Deutsch (Standard)](nachweis-statt-selbsteinschaetzung.md) | English

- Status: Draft
- Maintainer: maintainer team (reviews changes)
- Content checked: 2026-09-22 against the project rules and documentation structure of this repository; no practical use has been proven.
- Next review trigger: before team adoption and when practical feedback arrives
- Evidence of practical use: None; not marked as proven.
- Adoption: Decision of the adopting team.
- Use cases: None yet.

Maintenance and formats: [Documentation structure](../README.en.md).

## Problem

AI agents phrase results convincingly even when they are unchecked or incomplete.
Missing information is easily filled in plausibly, and sources or test results
are invented. Anyone relying on such statements adopts errors unchecked.

## Audience

Everyone who commissions, reviews, or passes on results from AI agents, whether
code, documentation, analyses, or research.

## Roles

- **AI agent:** supports statements with observations and marks unknowns.
- **Responsible person:** checks the evidence before passing on or approving a
  result.
- **Reviewer:** checks whether the evidence supports the statements.

## Process

### 1. Define the completion criterion in advance

Before the work, a verifiable criterion is agreed, such as a test, a command with
an expected result, or observable behavior.

### 2. Report observations, not assessments

A completion report states what was checked and with which result: command and
result, test name and outcome, observed file, or visible behavior. "Should work"
is not evidence.

### 3. Mark unknowns

Missing information is marked as `UNKNOWN: …` instead of being filled in. Sources,
URLs, numbers, and evidence of experience are never invented; a source is named
only if it was actually retrieved in the same working session.

### 4. State failures and limits openly

Failed checks are reported with their number and cause. Checks not performed and
the limits of a substitute check are named. A formal check does not prove
practical use.

## Templates

```text
Result: [what was achieved]
Evidence: [command/test/observation and result]
Not checked: [what remained open and why]
UNKNOWN: [missing information, if any]
```

## Limits

- The standard does not specify how thoroughly to check; the team decides based
  on risk.
- Evidence can itself be flawed; human review remains necessary.
- Adaptation points: minimum checks per type of change, form of the completion
  report.

## Sources

- Derived from the [project rules](../../AGENTS.en.md) and the verification
  standard in the [documentation structure](../README.en.md) of this repository.
- Proposal without proven practical use.

## Change history

- 2026-09-22: Created as a standard.
