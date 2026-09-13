# Security policy

## Do not report a vulnerability in a public issue

A public issue is readable by everyone the moment it is opened, including anyone
who might use the flaw. It stays readable in the history even after an edit or a
delete. Reporting a vulnerability that way puts every customer running the app at
risk before a fix exists.

## Report it privately instead

**Email <mira.maty@web.de>** and put *security* in the subject line.

GitHub's private vulnerability reporting is also enabled on this repository, if
you prefer it: open the **Security** tab and choose **Report a vulnerability**.
That opens a private thread visible only to you and to Matify.

## What to include

Enough to reproduce the issue, and no more than that:

- Which app, and which version — the **Diagnostics** tab shows both
- What an attacker could do, and what they would need in order to do it
- The steps, or a proof of concept
- Whether you have disclosed it anywhere else

You do not need to send a working exploit against a live site, and please do not
test against a site that is not your own.

## What happens next

Matify is a small publisher, so there is no round-the-clock security desk. What
you can expect is an acknowledgement that a person has read the report, an
assessment of whether it is exploitable and how far it reaches, a fix released
through the Atlassian Marketplace, and credit in the release notes if you would
like it.

Please give a reasonable window for a fix to ship before disclosing publicly.
The apps are Atlassian Forge apps, so a fix reaches every installation through
Atlassian rather than requiring customers to upgrade one by one — which usually
makes that window short.

## Scope

In scope: the Matify apps listed in the [README](README.md), and the public pages
at `matify25.github.io/matify-public`.

Not in scope: Atlassian's own platform, Jira Cloud itself, and the Forge runtime.
Report those to Atlassian at <https://www.atlassian.com/trust/security/report-vulnerability>.

## What the apps are built not to do

Context that may save you time. Access Auditor for Jira declares no write scope
of any kind, declares no external egress — Atlassian Forge blocks any outbound
request an app has not declared, so it is enforced by the platform rather than by
the code — and holds no API token, OAuth secret or other credential, because it
talks to no service outside Atlassian.

The full statement, with the evidence for each claim, is at
<https://matify25.github.io/matify-public/apps/access-auditor-for-jira/security-privacy/>.
If you find something that contradicts it, that itself is worth reporting.
