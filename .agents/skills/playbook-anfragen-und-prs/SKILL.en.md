# Change requests and pull requests

[Deutsch (Standard)](SKILL.md) | English

The German `SKILL.md` is the executable, authoritative skill entry point.

Read [Documentation structure and maintenance](../../../docs/README.en.md). Check
existing requests and changes to avoid creating a second record for the same
need. Before adopting decisions from linked issues or PRs, read their description
and every comment thread; state when access is incomplete.

## Change request

Use the [change request template](../../../docs/vorlagen/aenderungsanfrage.en.md).
Describe the problem, desired state, boundaries, and observable acceptance
criteria. Record ownership, decision, and next step. Use relative links while no
real GitHub record exists. Store a requested local change under the agreed path,
or under `docs/` if no path was specified. Public requests are a German default
plus an English `.en.md` version that link one another and share one decision state.

## Pull request

Use the [PR template](../../../docs/vorlagen/pull-request.en.md). The title names
the specific change and affected content. The description explains purpose,
resulting behavior, scope, and observed verification evidence. For public
content, name the verification of both languages. Update the title and body to
match the final scope.

Link the underlying request. Use closing syntax such as `Closes #…` only for a
real issue fully resolved by the PR. Record open follow-up work separately and
link it in both directions; retain rejections with a reason. When applying the
[team process](../../../docs/entwuerfe/teamprozess-mensch-ki-github.en.md), follow
its review ownership, commit reference, and follow-up rules.

Without a configured remote, provide a local PR draft. A real PR requires a
separate request and publishable changes; obtain explicit approval before every
commit. Do not create a remote, commit, or push to fill missing prerequisites
without authorization. A formatting request alone does not authorize external
creation.

Before delivery, check links and evidence. Never claim checks that did not run or
a PR URL before a PR exists.
