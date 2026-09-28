# Security policy

This policy applies to every public Alteriom repository that doesn't have its own `SECURITY.md`.

## Reporting a vulnerability

**Please don't report security vulnerabilities through public issues, discussions or pull
requests.**

Report them privately through GitHub instead:

1. Go to the affected repository's **Security** tab.
2. Click **Report a vulnerability**.
3. Fill in the advisory form.

Private vulnerability reporting is enabled on all our public repositories. If you can't use it,
email **admin@alteriom.ca** with "Security" in the subject line.

Please include as much of the following as you can:

- The affected repository, and the version, release or commit
- The type of issue (for example buffer overflow, authentication bypass, injection)
- The hardware and framework versions, for firmware issues
- Step-by-step instructions to reproduce the issue
- Proof-of-concept code, if you have it
- The impact, and how an attacker might exploit it

## What to expect

| Step | Target |
|---|---|
| Acknowledge your report | Within 5 business days |
| Initial assessment | Within 10 business days |
| Fix or mitigation | Depends on severity and complexity; we'll keep you updated |
| Public disclosure | Coordinated with you, once a fix is available |

We'll credit you in the published advisory unless you'd rather stay anonymous.

## Supported versions

Security fixes are made against the latest release of each project. Please check that you can
reproduce the issue on the latest release before reporting it.

## Scope

In scope: the code and published packages from public Alteriom repositories.

Out of scope:

- Vulnerabilities in third-party dependencies that are already publicly known (please report those
  upstream)
- Issues that require physical access to a device, unless the project claims to protect against it
- Denial of service by flooding a radio or network you control
- Social engineering

Some projects document known security limitations in their own `SECURITY.md`. painlessMesh, for
example, describes the limits of its security model. Please check the repository's documentation
before reporting.
