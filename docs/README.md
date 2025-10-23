# .github Documentation Hub

This directory provides organization-wide guidance for shared GitHub resources (profile README, issue templates, workflows, automation scripts, and badge usage). It intentionally excludes unverifiable marketing claims.

## Purpose

* Centralize maintenance notes for the public `.github` repository.
* Explain structure and conventions used in profile and automation.
* Provide contributors with clear expectations for updates.

## Directory Structure

```text
.github/
  profile/        # Organization public profile README
  docs/           # This documentation hub
  workflows/      # (Add shared GitHub Actions here if/when needed)
  ISSUE_TEMPLATE/ # (Add or refine templates; keep concise & actionable)
```

## Profile README Maintenance

| Aspect | Guideline |
|--------|-----------|
| Public repos table | Only include repositories actually public; update quarterly |
| Badges | Use shields.io factual badges (license, issues, last commit); avoid vanity metrics |
| Internal references | Clearly mark excluded internal repos; do not leak private paths |
| Custom badges | Only add if value is generated in a public artifact (e.g., docs audit JSON) |
| Roadmap | Use observed public analysis documents; avoid speculative feature lists |

### Adding/Removing Repositories

1. Confirm repository visibility (public vs internal).
2. If making public, ensure: LICENSE, README, basic issue template, code of conduct.
3. Update the profile table with concise focus & capabilities (max ~120 chars in capabilities cell).
4. Run markdown lint after edits.

## Badges Usage

Prefer minimal, factual badges: license, issues, last commit, top language, repo size (for config). Avoid chain rows of >12 badges.

Example syntax:

```markdown
![repo license](https://img.shields.io/github/license/Alteriom/repository-metadata-manager)
```

Custom badge placeholders should be rendered from scripts rather than hard-coded where possible.

## Automation (Planned / Optional)

If adding shared workflows:

* Use re-usable workflow calls from internal repos only after sanitizing secrets.
* Name workflows `org-docs-audit.yml`, `org-link-check.yml`, etc.
* Keep workflow concurrency limited to avoid rate limiting.

## Documentation Quality Scoring (Future)

Potential automated badge: `Docs Quality` produced by a script that aggregates coverage (examples, troubleshooting, specs alignment). Must output a JSON file with fields:

```json
{
  "coverage_examples": 0.72,
  "coverage_troubleshooting": 0.55,
  "structure_score": 0.81,
  "overall": 0.69
}
```

A script can convert `overall` to a shield via a dynamic endpoint or a manually updated badge.

## Contributor Expectations

* Keep changes small and reviewable.
* Explain rationale for adding any new badge or section.
* Avoid duplication of internal repository documentation.
* Reference issue numbers when removing or updating sections.

## Update Cadence

| Task | Frequency | Owner | Notes |
|------|-----------|-------|-------|
| Public repo snapshot refresh | Quarterly | Maintainer | Validate visibility before listing |
| Badge accuracy audit | Monthly | Maintainer | Ensure no broken badge endpoints |
| README lint & link check | Monthly | Maintainer | Add link checker workflow when available |
| Docs quality score (if implemented) | Monthly | Script/Workflow | Auto-update badge |

## Future Improvements

* Add link-check GitHub Action.
* Automate generation of the public repository table.
* Introduce dynamic badge for docs quality.
* Provide translation guidelines if localization begins.

---
**Last updated:** 2025-10-23
