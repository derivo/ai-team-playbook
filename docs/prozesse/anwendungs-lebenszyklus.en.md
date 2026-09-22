# Lifecycle of shared applications

[Deutsch (Standard)](anwendungs-lebenszyklus.md) | English

- Status: Draft
- Maintainer: maintainer team (reviews changes)
- Content checked: 2026-09-22 derived from the use case; no practical use has been proven.
- Next review trigger: before team adoption and when practical feedback arrives
- Evidence of practical use: None; not marked as proven.
- Adoption: Decision of the adopting team.
- Use cases: [App lifecycle in a company](../anwendungsfaelle/gedankenspiel-app-lifecycle.en.md)

Maintenance and formats: [Documentation structure](../README.en.md).

## Problem

With AI agents, small applications are built quickly. Once others use them, they
need support, data ownership, and eventually an orderly end. Without a defined
lifecycle, duplicate applications appear, experiments silently become
indispensable tools, and nobody feels responsible for outages or retirement.

## Audience

Teams and organizations in which people, alone or with AI agents, build
applications for shared use. The effort depends on significance: a limited
experiment needs less coordination than an application others depend on.

## Roles

- **Business owners:** own the benefit and business decisions.
- **Technical support with a deputy:** looks after technology, updates, and
  incidents.
- **Contact for new ideas:** classifies ideas together with the business owners.
- **Affected teams and specialists** (such as operations, IT security, or data
  protection): are involved when data, access, operations, or dependencies
  require it.
- **AI agents** can carry out work but do not take on organizational
  responsibility.

## Process

### 1. Make the idea visible

Before building for shared use, create an entry in the central application
directory. The entry persists throughout the lifecycle; development tasks and
changes are linked to it. It answers:

- Which problem should be solved, and for whom?
- Is there an existing application or a suitable extension option?
- Who takes business ownership?
- Which data, interfaces, and teams are affected?
- How will we know the application is worthwhile?

### 2. Classify

The contact reviews the idea with the business owners and involves those
affected. Outcome: use an existing solution, extend an existing solution, start a
limited trial, or defer the idea. The decision and its reason are recorded in the
entry.

### 3. Run a limited trial

A trial has owners, a small user group, and a date for deciding whether to
continue or stop. It is marked as an experiment. A personal trial with test data
can start in a simplified way. As soon as others are to use it regularly, real
data is connected, or a workflow depends on it, the classification from step 2 is
required.

Done when: stopped, continued with a new goal and date, or prepared for regular
operation.

### 4. Explicitly take over operation

Before regular use, the questions of the handover checklist are answered. Business
owners and technical support confirm the handover. Without named support, the
application remains a limited trial.

### 5. Decide on continuation regularly

At the review date, usage, benefit, costs, open issues, and support effort are
considered. Decision: continue, improve, merge with another solution, or retire.
Owners and the next review date are updated. If a supporting person leaves the
team, the handover is organized explicitly.

### 6. Retire in an orderly way

Users and dependent teams receive a retirement date and, if available, an
alternative. Required data is transferred or exported; remaining data is retained
or deleted according to applicable rules. Then jobs, integrations, access,
operation, and paid services are ended, and sources and documentation are
archived. The directory entry remains with the retirement date and successor.

## Templates

### Handover checklist

| Topic | Required answer |
|---|---|
| Ownership | Who owns the benefit and business decisions? |
| Support | Who looks after technology, updates, and incidents; who deputizes? |
| Location | Where are sources, documentation, and the directory entry? |
| Operation | Where does the application run, who bears costs and manages access? |
| Data | Which data is processed, who gets access, how is it retained or deleted? |
| Outage | How is an outage noticed, who responds, how does work continue meanwhile? |
| Recovery | If data or state must be preserved: how is it backed up and restored? |
| Usage | Who uses the application, and where are problems reported? |
| End | When is the benefit reviewed again, and how can the application be replaced? |

### Directory entry

```text
Name and purpose:
Status: Idea / Experiment / In preparation / In operation / Being replaced / Retired
Business owner:
Technical support and deputy:
User group:
Sources and documentation:
Data and dependencies:
Operating location and running costs:
Next decision, responsible person, and date:
```

## Limits

- The process does not replace legal, security, or data protection requirements;
  it only ensures that the responsible parties are involved in time.
- Adaptation points: location of the application directory, threshold for
  classification, review cadence (for example quarterly as a starting value), and
  the specialists involved.
- Success criterion for a trial: for every recorded application, it is possible
  to determine without asking why it exists, who supports it, what status it has,
  and when the next decision is due.

## Sources

- Derived from the use case
  [App lifecycle in a company](../anwendungsfaelle/gedankenspiel-app-lifecycle.en.md).
- Proposal without proven practical use.

## Change history

- 2026-09-22: Derived from the use case as a general process.
