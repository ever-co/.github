# Security Policy

Thank you for helping keep Ever® products and their users safe. This policy
covers every repository of the [ever-co](https://github.com/ever-co)
organization that has no `SECURITY.md` of its own: the code, the Docker images
and packages we publish from it, and the websites and services we run from it
(for example ever.co, everdemand.co, traduora.co and the docs sites of
these products). A repository with its own `SECURITY.md` follows that file
instead.

## Supported versions

Security fixes are made on the `develop` branch and ship with the next
release. We support the latest release and the `develop` branch. Older
releases do not get fixes: please upgrade to the latest.

## Reporting a vulnerability

**Please do not report security vulnerabilities in public GitHub issues,
discussions or pull requests.**

Report them privately, in one of these two ways:

1. **GitHub private vulnerability reporting (preferred):** open the
   repository's **Security** tab and choose **Report a vulnerability**
   (`https://github.com/ever-co/<repository>/security/advisories/new`). Only
   you and the maintainers can see the report, and we can discuss it, prepare
   the fix in a private fork and publish the advisory from the same place.
2. **Email:** <mailto:security@ever.co>.

Please include as much of the following as you can:

- the affected repository, component (API endpoint, web page, app, package,
  Docker image, website) and version or commit;
- the type of issue (for example authentication bypass, missing authorization
  or tenant isolation, injection, XSS, SSRF, secret exposure);
- step-by-step instructions to reproduce it, with a proof of concept if you
  have one;
- the impact: what an attacker can do, and what access they need first;
- any configuration the issue depends on.

Please test only against your own installation (for example a local
`docker compose` stack). Do not test against our hosted services or other
people's data, and do not run denial-of-service, spam or social-engineering
tests against our services or staff.

## What happens next

- We aim to acknowledge your report promptly, and we keep you updated while we
  investigate and fix it.
- We fix confirmed issues, release the fix, and publish a GitHub Security
  Advisory (with a CVE when one applies) once a fixed release is available.
- We credit reporters in the advisory, unless you ask us not to.
- Please keep the details private until the advisory is published.

Our websites also publish this contact in
[`/.well-known/security.txt`](https://ever.co/.well-known/security.txt)
(RFC 9116).
