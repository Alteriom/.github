# Security Policy

## Supported Scope

This policy applies only to the public repositories listed in `profile/README.md`.
Private or internal systems are out of scope for public disclosure.

## Reporting a Vulnerability

1. Do NOT open a public issue for undisclosed vulnerabilities.
2. Email: `security@alteriom.example` (placeholder; replace with operational address when available).
3. Provide: repository name, affected files, impact overview, reproduction steps.
4. Allow at least 14 days for triage and initial response.

## Vulnerability Classes in Scope

* Schema validation bypass (e.g., incorrect TypeScript definitions allowing unsafe payloads)
* Documentation conversion script injection (malicious input producing unsafe output)
* Metadata normalization producing unintended privilege escalation (if automation expands in scope)

## Out of Scope

* Cosmetic issues (typos, formatting)
* Vulnerabilities requiring access to private repositories
* Social engineering attacks

## Remediation Process

1. Triage & confirm.
2. Assign severity (Low / Moderate / High).
3. Develop fix and tests.
4. Publish advisory and patch simultaneously.
5. Credit reporter unless anonymity requested.

## Disclosure Timeline (Target)

| Step | Target Time |
|------|-------------|
| Acknowledge report | 5 business days |
| Initial triage     | 10 business days |
| Fix development    | 30 calendar days (depends on severity) |
| Advisory publish   | With patch release |

## GPG / Encryption

(Encryption key to be published here once available.)

## Versioning & Tags

Security fixes should increment patch version and reference CVE or internal advisory ID.

---
**Last updated:** 2025-10-23
