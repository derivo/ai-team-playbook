# Standard: Data and confidentiality when using AI

[Deutsch (Standard)](daten-und-vertraulichkeit.md) | English

- Status: Draft
- Maintainer: maintainer team (reviews changes)
- Content checked: 2026-09-22 written as a proposal; no practical use has been proven.
- Next review trigger: before team adoption and when practical feedback arrives
- Evidence of practical use: None; not marked as proven.
- Adoption: Decision of the adopting team.
- Use cases: None yet.

Maintenance and formats: [Documentation structure](../README.en.md).

## Problem

Working with AI tools means giving them content: code, documents, customer data,
credentials in configuration files. Without clear rules, it is unclear which data
may go to which tool. Confidential or personal data can reach third parties
unintentionally.

## Audience

Teams and organizations using AI tools with access to their own or others' data.
The standard provides the structure; the adopting team defines the specific data
classes and tools.

## Roles

- **Team:** defines data classes and approved tools.
- **Responsible specialists** (such as data protection or IT security): are
  involved in the definition and in case of doubt.
- **Users:** check which data class is affected before passing data to a tool.
- **AI agent:** passes data only to approved tools and reports detected
  credentials or personal data.

## Process

### 1. Define data classes

The team defines a few understandable classes, for example: public, internal,
confidential, personal, credentials.

### 2. Map tools

For each AI tool in use, record which data classes it is approved for, where data
is processed, and whether it may be stored or used for training. The basis is
the provider's verified terms, not assumptions.

### 3. Check before passing data on

Before pasting or sharing content, check whether the data class is approved for
the tool. When in doubt, do not pass it on and ask the responsible party.

### 4. Protect credentials

Credentials do not belong in prompts, code, documentation, or version control,
but in designated stores such as environment variables or secret stores. Changes
are checked for credentials and real personal data before a commit. An
accidentally shared secret is replaced, not merely deleted.

### 5. Report incidents

If data reaches a tool that is not approved, report it to the responsible party.

## Templates

| Tool | Approved data classes | Processing location | Storage/training | Checked on |
|---|---|---|---|---|
| [name] | [e.g. public, internal] | [region/provider] | [according to verified terms] | [date] |

## Limits

- The standard is not legal advice and does not replace legal, contractual, or
  data protection requirements.
- It deliberately contains no specific tool mapping, because that depends on the
  provider, contract, and context.
- Adaptation points: data classes, tool list, responsible parties, incident
  reporting channel.

## Sources

- Proposal without proven practical use. The credentials rule matches the
  verification standard in the [documentation structure](../README.en.md) of this
  repository.

## Change history

- 2026-09-22: Created as a standard.
