# Team process: Issues, pull requests, and AI reviews

[Deutsch (Standard)](teamprozess-mensch-ki-github.md) | English

- Status: Draft
- Maintainer: maintainer team (reviews changes)
- Content checked: Initial draft adopted; no practical use has been proven.
- Next review trigger: before team adoption and when practical feedback arrives
- Evidence of practical use: None; not marked as proven.
- Adoption: The adopting team decides; the following rules are a proposal.
- Examples: Illustrative and fictional; they are not documented experience.
- General process: [Collaboration between people and AI agents](../prozesse/zusammenarbeit-mensch-ki.en.md); this use case is a specific implementation of it.

Maintenance and formats: [Documentation structure](../README.en.md).

Updated process proposal for team discussion.

## Goal and basic rules

Everyone on the team can see who is working on what, whether a pull request (PR)
exists, and who needs to act next. Claude Code continues to run locally on team
members' computers. GitHub is the shared work overview.

- Every task has a responsible person, even when Claude implements it.
- The task is visibly claimed before work begins.
- Every handoff names a specific person and the next step.
- Automated reviews provide findings; human approval remains required.

## Process

### 1. Claim the task

Before starting Claude, use an existing GitHub issue or create one. Briefly state
the goal and completion criterion. Check whether somebody is already working on
it. The responsible colleague assigns themselves and sets the state to **In
progress**. If no PR exists, the issue explicitly says **No PR yet**.

### 2. Brief Claude

The colleague gives Claude the issue, goal, and scope boundaries. Claude checks
existing linked PRs so it does not duplicate implementation. The responsible
colleague clarifies ambiguous requirements.

### 3. Make work visible early

As soon as initial changes exist, Claude creates a **draft PR** and links it to
the issue. The draft makes active work visible; it is not yet a review request.

### 4. Keep status current

Update the status block in the issue when work starts, pauses, becomes blocked,
or is handed over. Claude should do this; the responsible colleague checks it no
later than when interrupting their work.

For a blocker, record what is missing and who must act next. Include the date and
time of the update: an old “In progress” entry does not prove that an agent is
still running.

### 5. Hand over for review

After the agreed checks, the responsible colleague reviews the result and its
verification evidence. They mark the PR ready for review and request a specific
colleague as reviewer. The issue says **Waiting for review**, including the
reviewer and next step.

Every AI review is visibly claimed on the PR before it starts and is accompanied
according to the review process below. The issue links to this review record.

Automated review findings are evaluated and either addressed or rejected with a
reason. When changes are requested, the next step returns to the author. The
author asks Claude to revise the work, runs the checks again, and then requests a
new review.

### 6. Complete the task

After human approval and successful project checks under the team rules, merge
the change. Before closing the original issue, create separate GitHub issues for
all concrete, identified follow-up work that remains open.

- Each follow-up issue describes the open point, relevant context, and reason for
  the follow-up. Link related review comments or decisions.
- The original issue links every follow-up issue. Each follow-up issue links back
  to the original issue and associated PR. This preserves the decision chain.
- Close the original issue only after all open follow-up work has been recorded
  and linked. This does not mean the follow-up work is complete.
- Reviewers may decide that a recorded follow-up is unnecessary. In that case,
  close the follow-up issue with a short reason. Do not delete it; retain the
  context and decision.

Identified follow-up work therefore does not remain only in comments, chats, or
local agent sessions. Linked issues keep it visible until it is implemented or
explicitly rejected.

## Claiming and tracking AI reviews

The task state remains in the issue. The concrete code review is documented on
the PR because it refers to a specific commit. A link in the issue points to the
current review record. This avoids maintaining review details in two places.

### Before the review

The colleague or automation checks whether somebody has already claimed a review
for this PR and commit. Before starting, create a review record containing the
responsible person, agent/session, reviewed commit, and start time. Also record
when the next update is expected.

First clarify an existing or unclear run with its owner. Start another independent
review only deliberately and label it as such.

### During the review

The agent or its accompanying automation regularly updates the review record with
the latest response and a brief progress note. Ten minutes between updates is an
initial guideline to test.

If an expected update does not arrive, monitoring independent of the review agent
checks the run, marks it **Check state**, and notifies the responsible colleague.
A crashed agent cannot reliably report its own failure. Until this monitoring is
implemented, the named colleague checks at the agreed time; there is no automatic
notification.

### When blocked or interrupted

Document a known blocker with its cause and next step. A late update only means
that the state is unclear; it does not automatically mean the run stopped.

Before resuming or replacing a run, determine whether the earlier run is still
working. Preserve already reviewed areas, findings, and open review points in the
existing record. The new run links to it and reuses the available interim state.
Explicitly record an interrupted run as interrupted; it is not a completed review.

### On completion

Link the published review result. The record names the commit actually reviewed
and whether the review was complete. New commits are not automatically covered
by an earlier review; the responsible reviewer decides which checks must be
repeated. Human approval remains required.

### Optional filtering labels

The review record is required. If the team also wants to filter by review state,
it uses this small label set on the PR. The labels describe one authoritative AI
review run; remove earlier state labels when the state changes.

| Label | Meaning |
| --- | --- |
| `review:ki-laeuft` | Review claimed and reported as running |
| `review:ki-blockiert` | Known blocker reported |
| `review:ki-pruefen` | Update overdue or run state unclear |
| `review:ki-abgebrochen` | Run ended with an incomplete review; interim state documented |
| `review:ki-fertig` | Complete result published for the named commit |

Labels alone do not prevent simultaneous starts. If several automations can start
reviews, a central assignment mechanism must ensure that only one regular run
claims a PR and commit. Until then, the responsible colleagues coordinate before
starting.

### PR review record template

```text
Responsible colleague: Ben
Agent/session: [unique identifier for the review run]
Reviewed commit: [commit ID]
Review state: Running / Blocked / Check state / Interrupted / Complete
Started: [date and time]
Last update: [date and time]
Next update expected by: [date and time]
Interim state: [areas checked, findings so far, open review points]
Next step and responsible person: [...]
Result or previous run: [link, if available]
```

## Shared status values

| State | Meaning |
| --- | --- |
| Open | Not claimed |
| In progress | A colleague is working on the task, possibly with Claude |
| Paused | Work deliberately interrupted |
| Blocked | A concrete prerequisite or decision is missing |
| Waiting for review | A named reviewer must act next |
| Being revised | The author is addressing review feedback |
| Done | Changes merged and issue closed |

## Status template for the issue description

Keep this block current so nobody needs to search the comment history.
“Responsible” names the task owner. “Next step” names the person who must act now.

```text
Responsible: Anna
Agent: Anna's local Claude Code
State: Waiting for review
PR: [link or “No PR yet”]
AI review: [link to current review record or “Not started”]
Next step: Ben reviews the changes.
Blocker: None
Last updated: [date and time]
```

## Introduction

First trial the process with two colleagues on one task. Success criterion: an
uninvolved colleague can use the issue to identify the owner, associated PR,
work state, and next responsible person without asking questions.

For the first trial, status maintenance and claiming may be manual. Also simulate
an interrupted AI review: the responsible colleague must notice the missing
progress and understand the previous state before starting a replacement run.

Automated updates, monitoring, and notifications require separate setup. The
labels and templates above do not provide those functions by themselves.
