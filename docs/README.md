# Maintainer guide

How to keep the organization profile and the default community health files accurate.

## The one rule

**This repository is public.** Only public repositories, published packages and public URLs belong
here. Internal repository names, hostnames, IP addresses, agent names and infrastructure details
belong in the members-only `.github-private` repository.

## Updating the profile

[`profile/README.md`](../profile/README.md) groups projects into four areas:

| Section | Projects |
|---|---|
| Mesh networking & device libraries | painlessMesh, LoRa E220 library, painlessMesh-simulator |
| Telemetry & integration | mqtt-schema, webhook-client (TypeScript and Python) |
| Hardware-in-the-loop testing | esp32-rig, esp32-hil-firmware, esp32-rig-example |
| Build & developer tooling | docker-images, repository-metadata-manager, ai-dev-skills |

Update it when:

- a repository is made public, archived, renamed or deleted;
- a project changes its package name, registry or documentation URL;
- a project's one-line description no longer matches what it does.

Version badges come from shields.io and update themselves, so a new release doesn't need a profile
change.

To list the current public repositories:

```bash
gh repo list Alteriom --visibility public --no-archived --json name,description --limit 100
```

### Writing style

- One or two sentences per project: what it does and who it's for.
- Only claim what a visitor can verify from the repository itself.
- Link to the package registry or docs site where one exists.
- Use badges only for version and release; they must be generated from public data.

## Before making a repository public

- [ ] `LICENSE` file present
- [ ] README explains what the project is, how to install it and how to use it
- [ ] Repository description and topics set (`gh repo edit --description ... --add-topic ...`)
- [ ] No secrets, internal hostnames or IP addresses in the code **or in the git history**
- [ ] Private vulnerability reporting enabled (Settings → Code security)
- [ ] Added to `profile/README.md`

## Default community health files

GitHub uses `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`, `SUPPORT.md`, the issue forms
and the pull request template from this repository for any public repository that doesn't have its
own. Keep them generic: they must make sense for a C++ firmware library and for a TypeScript SDK
alike.

The security and code-of-conduct contact is **admin@alteriom.ca**, the organization's public email.
If it changes, update `SECURITY.md` and `CODE_OF_CONDUCT.md` together.

## Review cadence

| Task | When |
|---|---|
| Check the profile against the list of public repositories | Every quarter, and whenever visibility changes |
| Check links and badges in the profile | Every quarter |
| Review default health files | Once a year |

---

**Last updated:** 2026-09-28
