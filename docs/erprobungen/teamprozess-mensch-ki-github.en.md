# Trial: Team process with GitHub and local Claude clients

[Deutsch (Standard)](teamprozess-mensch-ki-github.md) | English

- State: Prepared
- Maintainer: maintainer team (reviews changes)
- Use case under trial: [Team process with GitHub and local Claude clients](../anwendungsfaelle/teamprozess-mensch-ki-github.en.md)
- General process: [Collaboration between people and AI agents](../prozesse/zusammenarbeit-mensch-ki.en.md)
- Period: UNKNOWN: start and end
- Result: None yet; both documents remain Draft until the evaluation.

Maintenance and formats: [Documentation structure](../README.en.md).

## Goal and questions

The trial checks whether the use case works in a real team:

1. Can an uninvolved person identify the owner, the linked pull request, the
   work state, and the next responsible person from the issue alone?
2. Is an interrupted AI review noticed, and can its previous state be traced
   before a replacement run?
3. Is the effort of maintaining the status block and review record sustainable
   in daily work?

Questions 1 and 2 come from the "Introduction" section of the use case. Question 3
adds the effort, which is decisive for team adoption.

## Context

- Team: UNKNOWN: team or organizational unit
- Repository: UNKNOWN: GitHub repository used for the trial
- Participants: UNKNOWN: two people, each with their own local Claude Code
- Uninvolved person for the evaluation: UNKNOWN: a person who works on neither
  the task nor the review
- Task: UNKNOWN: a real, manageable change with a review

Enter names of real people in this public repository only with their consent;
otherwise use roles.

## Preparation

- [ ] Define the team, repository, participants, and uninvolved person.
- [ ] Define the period; two to four weeks is a proposal, not an experience value.
- [ ] Select a task that requires a pull request and a review.
- [ ] Read the use case with all participants and note team deviations in
      advance, such as state names or the update interval.
- [ ] Prepare the status block and review record from the use case. Status
      updates and task ownership are handled manually; labels, automations, and
      monitoring are not set up for the trial.
- [ ] Agree on who records the observations below.

## Procedure

### Scenario A: Task from ownership to completion

The participants work on the task following steps 1 to 6 of the use case: take on
the issue, instruct Claude, create a draft pull request, maintain the status,
hand over for review, complete, and record follow-up work as issues.

At least once during the work, such as at a pause or handoff, and once after
completion, the uninvolved person reads only the issue and answers question 1
without asking. The answers are compared with the actual state.

### Scenario B: Interrupted AI review

An AI review is started according to the section "Claiming and tracking AI
reviews" and deliberately aborted, for example by ending the Claude
session. The responsible colleague checks at the agreed time, notices the missing
update, records the run as aborted, and starts a replacement run that links to
the previous record.

## Observations

Record during the trial, with dates:

| Time | Scenario | Question | Uninvolved person's answer or observation | Matches the actual state? |
|---|---|---|---|---|
| [date] | A | 1 | [...] | Yes / No, because [...] |

Also record: places where the status block or review record was forgotten or
outdated, estimated maintenance effort, and deviations from the use case.

## Evaluation and result

UNKNOWN: to be completed after the trial.

- Which questions were answered with yes, which were not, and why?
- Which rules of the use case worked well, and which did not?
- Which changes to the use case or the general process follow from this?

## Limits

- Two people and one task do not prove that the process works in larger teams or
  with many parallel tasks.
- Without monitoring in place, automatic detection of missing updates is not
  tested, only the manual check.
- The result applies to the use case. For the general process, it is an
  indication but not complete evidence.

## Status decision

After the evaluation, the maintainer team decides whether the use case receives
the status `proven`. According to the
[documentation structure](../README.en.md), this requires documented context,
time, approach, result, and limits. A successful trial is recorded in the use
case header as evidence of practical use, linking to this document.

## Change history

- 2026-09-22: Trial prepared.
