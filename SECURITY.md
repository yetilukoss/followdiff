# Security Policy

## Reporting a vulnerability

If you find a security vulnerability in FollowDiff, please report it responsibly:

1. **Do not** open a public issue for security vulnerabilities.
2. Use GitHub's private vulnerability reporting: https://github.com/yetilukoss/followdiff/security/advisories/new
3. Or email the maintainer via GitHub (profile: https://github.com/yetilukoss)

We will respond within 7 days and work on a fix.

## What counts as a vulnerability

- Data leakage (your data being sent to a third party)
- Unauthorized access to your Instagram account
- Code injection or remote code execution
- Permission escalation beyond what's declared in the manifest

## What does not count

- Instagram changing their API and breaking functionality (not a security issue)
- Feature requests or UX issues (use regular issues)
- Third-party Instagram API behavior

## Scope

FollowDiff runs entirely in your browser. There is no backend, no server, and no database. The attack surface is limited to the extension code itself.
