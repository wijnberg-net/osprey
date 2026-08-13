# Security Policy

Osprey is proprietary software distributed as compiled packages through this
repository. The source code is not public, but security reports are welcome,
taken seriously, and handled through a coordinated disclosure process.

## Supported versions

Security fixes are delivered as new releases in this repository. Only the
**latest published release** receives security fixes. If you are on an older
version, please upgrade and re-test before reporting.

## Reporting a vulnerability

**Please do not report security issues in public GitHub issues.**

Preferred channel — GitHub private vulnerability reporting:

- [Report a vulnerability](https://github.com/wijnberg-net/osprey/security/advisories/new)
  (kept private between you and us until a fix is released)

Alternatively, email **security@wijnberg.net**. If you need an encrypted
channel, say so in your first mail and we will arrange one.

A useful report includes:

- Osprey version (`dpkg -s osprey | grep Version`, or the version shown in the
  web UI under Help → About)
- Deployment details (OS, install method, which services are affected —
  engine, api, collector-manager, snmp-poller, bmp-server, web UI)
- Reproduction steps or a proof of concept
- Your assessment of the impact

Please redact SNMP communities, credentials, and internal addressing from any
logs or captures you attach.

## What to expect

- **Acknowledgement within 3 business days.**
- A status update at least every 14 days while we investigate and fix.
- Coordinated disclosure: we ask that you keep the issue private for up to
  90 days or until a fixed release is published, whichever comes first.
- Credit in the release notes for the fix, unless you prefer to remain
  anonymous.

There is currently no bug bounty program; reports are handled on a
best-effort, good-faith basis and we will not pursue action against
researchers acting in good faith within this policy.

## Scope

In scope:

- The Osprey packages published under
  [Releases](https://github.com/wijnberg-net/osprey/releases) — all bundled
  services, the web UI, and the packaging/installation scripts they contain.

Out of scope:

- Vulnerabilities exclusively in third-party dependencies (please report
  upstream — but do tell us as well so we can ship the updated dependency).
- The wijnberg.net websites and mail infrastructure.
- Findings that require an already-compromised host or an operator with
  administrative access acting maliciously.
