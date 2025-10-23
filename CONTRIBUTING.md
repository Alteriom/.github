# Contributing Guide

Thank you for your interest in contributing to Alteriom's public repositories.

## Public Scope

Only contribute to repositories explicitly listed in the public table inside `profile/README.md`.
Do not reference or attempt to access private/internal repositories or unpublished tooling.

## Ground Rules

* Keep changes atomic and focused.
* Use clear commit messages (imperative tone, e.g., "Add schema diff helper").
* Add or update tests when altering schema, metadata normalization, or conversion scripts.
* Maintain existing file naming conventions (kebab-case for Markdown, lowercase directories).
* Avoid adding performance claims or metrics not publicly verifiable.

## Pull Request Checklist

Before submitting:

* [ ] Linked related issue (or created one if none existed)
* [ ] Added tests / updated existing tests
* [ ] Updated documentation (if applicable)
* [ ] Ensured LICENSE headers or file are present if new repo/file type added
* [ ] Ran markdown lint (`markdownlint`) locally (optional but encouraged)

## Schema Changes (`alteriom-mqtt-schema`)

1. Increment version where appropriate.
2. Provide a changelog entry (new section or update existing).
3. Include validation test for new/changed fields.
4. Ensure backward compatibility notes if breaking change.

## Metadata Normalization (`repository-metadata-manager`)

* Keep topic additions minimal and relevant.
* Document rationale for bulk metadata changes in PR description.
* Run build/test suite to confirm no regressions.

## Documentation Conversion (`alteriom-docker-images`)

* Provide example input and output in PR body for new conversion rule changes.
* Preserve original semantic meaning while normalizing formatting.
* Avoid embedding internal file paths.

## Security & Disclosure

* Do not post vulnerabilities publicly before coordinating via SECURITY.md process.
* Clearly mark security-related PRs with the `security` label.

## Review Expectations

Maintainers aim to review within 5 business days. Larger or complex changes may take longer.
Use draft PRs for early feedback.

## Communication

* Use Issues for feature requests or bug reports.
* Discussions (if enabled) for broader design questions.
* Keep tone constructive and respectful (see CODE_OF_CONDUCT.md).

---
**Last updated:** 2025-10-23
