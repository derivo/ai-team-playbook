# Thought experiment: From app idea to retirement

[Deutsch (Standard)](gedankenspiel-app-lifecycle.md) | English

- Status: Draft
- Maintainer: UNKNOWN: not assigned
- Content checked: Initial draft adopted; no practical use has been proven.
- Next review trigger: before team adoption and when practical feedback arrives
- Adoption: The adopting team decides; the following rules are a proposal.
- Examples: Illustrative and fictional; they are not documented experience.

Maintenance and formats: [Documentation structure](../README.en.md).

Discussion proposal for the team, not an adopted company policy.

## Starting point

A rapidly developed application still needs care after its first use. Every
shared app should therefore have a purpose, an owner, and a managed lifecycle.
The effort should reflect its importance: a limited experiment needs less
coordination than an application on which other teams depend.

## 1. Make the idea visible

Before building something for shared use, create a short idea record in a central
application directory. A shared GitHub Projects overview with one issue per app
can serve as an initial solution. The application issue remains throughout the
lifecycle; individual development tasks and PRs link back to it.

The idea record answers:

- Which problem should be solved, and for whom?
- Does an application or suitable extension already exist?
- Who takes business ownership?
- Which data, interfaces, and teams are affected?
- How will we know that the application is worthwhile?

## 2. Review and classify briefly

A named contact in the team reviews the idea with the business owner. Affected
teams participate; IT, operations, or privacy specialists join when data, access,
hosting, or dependencies require them.

The outcome is one of: use an existing solution, extend an existing solution,
start a limited trial, or defer the idea. Not every idea needs a large approval
round, but record the decision and its reason.

## 3. Allow a limited trial

An experiment receives an owner, a small user group, and a date for deciding
whether to continue or stop. It is marked as an experiment and does not silently
become a permanent work tool.

A personal trial with test data may start with fewer steps. As soon as other
people should use it regularly, real company data is connected, or a workflow
depends on it, the review from step 2 is required.

At the end of the trial, decide whether to stop, continue testing with a new goal
and date, or prepare for regular operation.

## 4. Explicitly accept operational responsibility

Before regular use, answer at least these questions:

| Topic | Required answer |
| --- | --- |
| Ownership | Who owns the benefit and business decisions? |
| Maintenance | Who handles technology, updates, and incidents, and who is the backup? |
| Location | Where are the repository, documentation, and application-directory entry? |
| Operation | Where does the app run, who pays its costs, and who manages access? |
| Data | Which data is processed, who can access it, and how is it retained or deleted? |
| Outage | How is an outage detected, who responds, and how does the team work meanwhile? |
| Recovery | If data or state must be retained, how is it backed up and restored? |
| Use | Who are the users, and where do they report problems? |
| End | When is value reviewed again, and how can the app be replaced? |

The business owner and technical maintainer confirm the handover. Without a named
maintainer, the application remains a limited experiment. An AI agent may perform
work but does not assume organizational responsibility.

## 5. Decide regularly whether to continue

At the agreed review date, consider usage, value, cost, open problems, and
maintenance effort. A quarterly review is a possible starting proposal; the team
adapts the cadence to the application.

The decision is to continue, improve, consolidate with another solution, or
retire. Update the owners and next review date. If the maintainer leaves the team,
organize an explicit handover.

## 6. Retire in an orderly way

Give users and dependent teams a retirement date and, where applicable, an
alternative. Transfer or export required data; retain or delete remaining data
under the applicable rules. Then stop jobs, integrations, access, hosting, and
paid services. Archive the repository and documentation appropriately.

Keep the directory entry with the retirement date and successor solution so that
nobody later rebuilds the same application unknowingly.

## Minimum record for each application

```text
Name and purpose:
Status: Idea / Experiment / Preparing / Operating / Being replaced / Retired
Business owner:
Technical maintainer and backup:
User group:
Repository and documentation:
Data and dependencies:
Operating location and recurring costs:
Next decision, responsible person, and date:
```

## Concrete example

A colleague wants to build a small app for preparing customer lists. She records
the idea, checks existing solutions, and coordinates the planned data use with
the responsible people. A time-limited trial starts with test data.

The trial shows sufficient value. Before more colleagues use the app regularly,
the team clarifies maintenance, access, operation, and outage handling. At a later
review, an existing system takes over the function. The data is transferred and
the app is retired in an orderly way.

## Starting in the company

Trial the proposal with one new idea and one small app already in use. First
select the shared location and the contact for new ideas.

Success criterion: for both applications, someone can determine without asking
why they exist, who maintains them, their status, and when the next decision is due.
