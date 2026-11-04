# Security Policy

This is the default security policy for every repository in the actions.fyi
organization. A repository that ships its own `SECURITY.md` replaces this
policy entirely.

## Supported Versions

Security fixes go to the latest release of a repository. A repository without
releases receives fixes on its default branch only. Older releases are not
patched unless the repository's own policy says otherwise.

## Reporting a Vulnerability

Please do **not** report vulnerabilities through public issues, pull requests
or discussions.

Report them privately instead: open the **Security** tab of the affected
repository and select **Report a vulnerability**. Only the maintainers can see
the report.

If that button is missing, open an issue that asks for a private contact. Do
not include any details of the vulnerability in it.

### Filling in the report

The report opens as a draft security advisory. Its fields are:

| Field | What to put in it |
| --- | --- |
| Title | One line naming the problem. |
| CVE identifier | Leave it empty. We request a CVE when we publish the advisory. |
| Summary | The problem in a few sentences, with its impact and severity. |
| Details | The full explanation. Links to the affected source lines help most. |
| Proof of concept | Complete steps to reproduce it, including any configuration they need. |
| Impact | The kind of vulnerability, and who is affected by it. |
| Affected products | The ecosystem, the package, and the affected and patched versions, as far as you know them. |
| Severity | A severity rating or CVSS vector, if you have one. "Unknown" is fine. |
| Weaknesses | The matching CWE, if you know it. |
| Credits | Anyone else who should be credited for the finding. |

You don't have to fill in every field or follow this layout strictly. A brief
report is welcome if it includes steps to reproduce the problem, or if the
vulnerability is obvious enough that it needs no explanation.

After you submit, the advisory's description is a single Markdown text that
you can keep editing. At that point you can also add a **Remedy** section with
the fix you suggest.

## What Happens Next

- We acknowledge the report within **7 days**.
- We send an initial assessment within **14 days**, and an update at least
  every **14 days** after that until the report is resolved.
- If we accept the report, we fix it, publish a GitHub Security Advisory and
  request a CVE where one applies. You are credited in the advisory unless you
  ask not to be.
- If we decline the report, we tell you why.

## Scope

In scope is the code and configuration published in actions.fyi repositories.

Out of scope:

- vulnerabilities in third-party dependencies or actions; please report those
  to their maintainers
- vulnerabilities in GitHub itself; please report those through
  [GitHub's bug bounty program](https://bounty.github.com/)

## Disclosure

We ask that you keep the vulnerability private until a fix is released, or
for **90 days** after your report, whichever comes first. We may agree on a
different date with you if a fix needs more time.

We will not pursue legal action against anyone who researches and reports a
vulnerability in good faith and in line with this policy.
