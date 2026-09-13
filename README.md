# Matify Marketplace App Support

Public support, bug tracking and feature requests for the Atlassian Marketplace
apps published by **Matify**.

You do not need to buy anything to open an issue here, and you do not need a
Jira administrator to do it for you. A GitHub account is the only requirement.

| | |
|---|---|
| **Ask a question or report a problem** | [Open an issue](https://github.com/Matify25/matify-support/issues/new/choose) |
| **See what is already reported** | [All issues](https://github.com/Matify25/matify-support/issues) |
| **Email support** | <mira.maty@web.de> |
| **Report a security vulnerability** | <mira.maty@web.de> — **never** as a public issue. See [SECURITY.md](SECURITY.md). |

## What this repository is

A ticket system, and nothing else. It holds no application source code — the
Matify apps are proprietary and are distributed only through the Atlassian
Marketplace.

That is deliberate. Support belongs somewhere a customer can search before
writing, read what other people have already asked, and follow a bug to the
version that fixes it. An email inbox does none of those things.

One tracker serves every Matify app, so you never have to work out which
repository a question belongs in. Each issue records which app it concerns.

## Supported apps

| App | Product | Documentation |
|---|---|---|
| **Access Auditor for Jira** | Jira Cloud | [Documentation](https://matify25.github.io/matify-public/apps/access-auditor-for-jira/docs/) |

Future Matify apps are added to this table and to the app selector on each issue
form. This tracker is the support channel for all of them.

### Access Auditor for Jira

Read-only permission auditing for Jira Cloud: who can access what, and why. It
resolves every project permission to the people and groups who actually hold it,
shows the chain of configuration that granted it, and reports the configurations
most likely to be a risk.

- [Documentation](https://matify25.github.io/matify-public/apps/access-auditor-for-jira/docs/)
- [Getting started](https://matify25.github.io/matify-public/apps/access-auditor-for-jira/docs/getting-started/)
- [Troubleshooting and error codes](https://matify25.github.io/matify-public/apps/access-auditor-for-jira/docs/troubleshooting/)
- [FAQ](https://matify25.github.io/matify-public/apps/access-auditor-for-jira/docs/faq/)
- [Known limitations](https://matify25.github.io/matify-public/apps/access-auditor-for-jira/docs/known-limitations/)
- [Security and privacy statement](https://matify25.github.io/matify-public/apps/access-auditor-for-jira/security-privacy/)
- [Privacy policy](https://matify25.github.io/matify-public/apps/access-auditor-for-jira/privacy/)

## Which form to use

**[Support request](https://github.com/Matify25/matify-support/issues/new?template=02-support-request.yml)** —
a question about how the app works, how to configure it, or how to read what it
reports. Also the right form for a question before buying.

**[Bug report](https://github.com/Matify25/matify-support/issues/new?template=01-bug-report.yml)** —
something behaves incorrectly or does not work. The form asks for steps,
expected behaviour and actual behaviour, because a report without those three
usually costs a round trip before anything can be investigated.

**[Feature request](https://github.com/Matify25/matify-support/issues/new?template=03-feature-request.yml)** —
something the app should be able to do and cannot. Worth reading
[known limitations](https://matify25.github.io/matify-public/apps/access-auditor-for-jira/docs/known-limitations/)
first: some absences are boundaries of what the Jira Cloud API exposes to any
app, not oversights, and that page says which.

Blank issues are turned off. Every form asks for the app, the version and the
site size, because those three change the answer often enough that a reply
without them would just be asking for them.

## Never post secrets here

**This repository is public.** Anything you write is readable by everyone, and
stays readable in the history after an edit or a delete.

Do not include passwords, API tokens, personal data, customer confidential data
or other secrets. Nothing on any form needs them.

Specifically, please leave out Atlassian account IDs, email addresses, real user
or customer names, Jira issue content, internal hostnames and URLs, and anything
your organisation would not publish on its own website.

If a problem genuinely cannot be described without one of those, email
<mira.maty@web.de> instead. Something posted here by mistake can be redacted on
request, but a public repository has readers and caches, so treat a slip as
disclosed and act accordingly.

### The diagnostic report is safe to post

Access Auditor's **Diagnostics** tab has a **Copy diagnostic report** button. That
report is built to contain no personal data and no credentials — no project name,
group name, account identifier or permission holder appears in it. Pasting it
into a bug report is encouraged: it answers most of what a first reply would
otherwise have to ask.

## Security vulnerabilities

**Never open a public issue for a suspected vulnerability.**

Email <mira.maty@web.de> with *security* in the subject line, or use GitHub's
private vulnerability reporting from the **Security** tab. Full policy in
[SECURITY.md](SECURITY.md).

## What to expect

Matify is a small publisher and support is handled by a person, not a rota.
Setting expectations honestly is more useful than a number nobody can keep:

- Issues are read on **business days**, Central European Time.
- A security report gets attention ahead of everything else.
- A bug report that arrives with steps, expected and actual behaviour, and a
  diagnostic report is usually answered on the first reply rather than the
  third. The forms ask for exactly those things for that reason.
- A question already answered in the documentation gets a link to it. That is
  not a brush-off — it is the fastest correct answer, and the page is kept
  current.

**No contractual response time is promised here.** Where a support commitment
exists it is the one on the Atlassian Marketplace listing and in the end user
terms, not this page. If you need a guaranteed response time, ask by email
before purchasing rather than assuming one.

Apps are distributed as Atlassian Forge apps, so a fix reaches every installation
through Atlassian. There is no upgrade for you to perform and no version for you
to chase.

## Labels

| Label | Meaning |
|---|---|
| `type: bug` · `type: support` · `type: feature` | What the issue is |
| `status: triage` | Received, not yet assessed |
| `status: confirmed` | Reproduced, or accepted as valid |
| `status: in progress` | Being worked on |
| `status: shipped` | Released to the Marketplace |
| `status: wont fix` | Deliberately not doing this — the issue says why |
| `status: not possible` | The Jira Cloud API does not expose what this would need |
| `app: access-auditor-for-jira` | Which app it concerns |

## Pull requests

This repository holds no code, so there is nothing to submit a pull request
against. Corrections to the documentation are welcome as an issue.

---

**Publisher:** Matify
**Support:** <mira.maty@web.de>

Copyright 2026 Matify. All Rights Reserved. The Matify apps are proprietary
software distributed through the Atlassian Marketplace; no source code is
published here or licensed by this repository.
