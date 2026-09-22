# Collaboration between people and AI agents on shared changes

[Deutsch (Standard)](zusammenarbeit-mensch-ki.md) | English

- Status: Draft
- Maintainer: maintainer team (reviews changes)
- Content checked: 2026-09-22 derived from the use case; no practical use has been proven.
- Next review trigger: before team adoption and when practical feedback arrives
- Evidence of practical use: None; not marked as proven.
- Adoption: Decision of the adopting team.
- Use cases: [Team process with GitHub and local Claude clients](../anwendungsfaelle/teamprozess-mensch-ki-github.en.md)

Maintenance and formats: [Documentation structure](../README.en.md).

## Problem

When several people each let their own AI agents work on shared changes, it is
often unclear who owns a task, whether someone is already working on it, whether
an agent is still running, and who has to act next. The results are duplicate
implementations, stalled reviews, and forgotten follow-up work.

## Audience

Teams that jointly produce changes to code, documentation, or other versioned
content and use AI agents while doing so. The process assumes a shared task
tracker and a review procedure for change proposals, such as pull or merge
requests. Tools and agents can be chosen freely.

## Roles

- **Responsible person:** owns the task, instructs the agent, clarifies
  requirements, and releases results for review. Every task has exactly one
  responsible person, even when an agent implements it.
- **Executing agent:** implements the task within the given scope and keeps the
  state current as far as the team delegates this to it.
- **Reviewer:** a named person who reviews and approves the change proposal.
  Automated reviews provide hints; human approval remains required.
- **Review agent:** an AI agent that reviews a change proposal. Every run has a
  responsible person.

## Process

### 1. Take on the task

Before starting, create the task in the shared task tracker or use an existing
one. Briefly describe the goal and the definition of done. Check whether someone
is already working on it. The responsible person assigns themselves and sets the
state to **In progress**.

Done when: the task names the owner, goal, definition of done, and state.

### 2. Instruct the agent

The responsible person gives the agent the task, the goal, and the limits of the
assignment. The agent checks existing linked change proposals to avoid duplicate
implementation. The responsible person clarifies unclear requirements.

### 3. Make work visible early

As soon as first changes exist, a change proposal marked as a draft is created
and linked to the task. A draft shows ongoing work; it is not yet a review
request.

### 4. Keep the state current

Update the task's status block at start, pause, blockage, and handoff. For a
blockage, record what is missing and who has to act next. Include the date and
time of the update: an old "In progress" entry does not prove that an agent is
still running.

### 5. Hand over for review

After the agreed checks, the responsible person verifies the result and the
verification evidence, marks the change proposal as ready for review, and names a
specific reviewer. The task is set to **Awaiting review**, including reviewer and
next step.

Hints from automated reviews are addressed or rejected with a reason. If changes
are requested, the next step returns to the responsible person; after revision,
checks are repeated and a new review is requested.

### 6. Track AI reviews

The task state stays with the task; the review record stays with the change
proposal because it refers to a specific version. The task links to the current
review record.

- **Before starting:** check whether a review is already running for this version.
  Create a review record with responsible person, agent/session, reviewed
  version, start time, and next expected update. An additional independent review
  is started only deliberately and marked as such.
- **During the review:** update the record regularly with the latest update and
  interim state. The team defines the interval.
- **Missing update:** a crashed agent cannot reliably report its own failure. A
  monitor independent of the agent or, without one, the responsible person checks
  the run at the agreed time. An overdue update means "state unclear", not
  automatically an abort.
- **Abort and replacement run:** before a replacement run, clarify whether the
  previous run is still working. Findings and open review points stay in the
  previous record; the new run links to it. An aborted run does not count as a
  completed review.
- **Completion:** the result is linked, stating the reviewed version and whether
  the review was complete. New changes are not automatically covered by an older
  review.

### 7. Complete and record follow-up work

After human approval and passing project checks, the change is merged. Before the
task is closed, every identified open follow-up item is created as its own task
with the open point, context, and reason. The original task and the follow-up
tasks link to each other. A follow-up item judged unnecessary is closed with a
reason, not deleted.

Done when: the change is merged, the task is closed, and every follow-up item is
visible as a linked task.

## Templates

### States

| State | Meaning |
|---|---|
| Open | Not yet taken on |
| In progress | A person is working on the task, possibly with an agent |
| Paused | Work deliberately interrupted |
| Blocked | A specific prerequisite or decision is missing |
| Awaiting review | A named reviewer acts next |
| In revision | The responsible person addresses review feedback |
| Done | Change merged and task closed |

### Task status block

```text
Responsible: [name]
Agent: [agent and where it runs]
State: [state]
Change proposal: [link or "None yet"]
AI review: [link to the review record or "Not started"]
Next step: [person and action]
Blocker: [cause or "None"]
Last updated: [date and time]
```

### Review record on the change proposal

```text
Responsible: [name]
Agent/session: [unique name of the review run]
Reviewed version: [identifier]
Review state: Running / Blocked / Check state / Aborted / Done
Started: [date and time]
Last update: [date and time]
Next update expected by: [date and time]
Interim state: [areas reviewed, findings, open review points]
Next step and responsible person: [...]
Result or previous run: [link, if available]
```

## Limits

- The process requires a shared task tracker and a review procedure; it does not
  replace project checks or approval rules.
- Monitoring, notifications, and assigning a review run to exactly one agent are
  adaptation points. Templates and states alone do not provide these functions.
- Without technical assignment, the responsible people coordinate before
  starting a review.
- Adaptation points: state names, update interval, location of the status block,
  optional labels for filtering.
- Success criterion for a trial: an uninvolved person can identify the owner,
  the change proposal, the state, and the next responsible person from the task
  without asking.

## Sources

- Derived from the use case
  [Team process with GitHub and local Claude clients](../anwendungsfaelle/teamprozess-mensch-ki-github.en.md).
- Proposal without proven practical use.

## Change history

- 2026-09-22: Derived from the use case as a tool-independent process.
