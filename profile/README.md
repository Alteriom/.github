# Alteriom Public Overview

> Baseline public information for Alteriom. This file intentionally excludes any private or internal repositories, tools, or unpublished metrics.

<!-- Core Public Repository Badges -->
![mqtt-schema license](https://img.shields.io/github/license/Alteriom/alteriom-mqtt-schema)
![mqtt-schema issues](https://img.shields.io/github/issues/Alteriom/alteriom-mqtt-schema)
![mqtt-schema last commit](https://img.shields.io/github/last-commit/Alteriom/alteriom-mqtt-schema)
![mqtt-schema top language](https://img.shields.io/github/languages/top/Alteriom/alteriom-mqtt-schema)

![metadata-manager license](https://img.shields.io/github/license/Alteriom/repository-metadata-manager)
![metadata-manager issues](https://img.shields.io/github/issues/Alteriom/repository-metadata-manager)
![metadata-manager last commit](https://img.shields.io/github/last-commit/Alteriom/repository-metadata-manager)
![metadata-manager top language](https://img.shields.io/github/languages/top/Alteriom/repository-metadata-manager)

![docker-images license](https://img.shields.io/github/license/Alteriom/alteriom-docker-images)
![docker-images issues](https://img.shields.io/github/issues/Alteriom/alteriom-docker-images)
![docker-images last commit](https://img.shields.io/github/last-commit/Alteriom/alteriom-docker-images)
![docker-images top language](https://img.shields.io/github/languages/top/Alteriom/alteriom-docker-images)

![org-config last commit](https://img.shields.io/github/last-commit/Alteriom/.github)
![org-config repo size](https://img.shields.io/github/repo-size/Alteriom/.github)

<!-- Fork / External references (read-only) -->
![painlessMesh fork](https://img.shields.io/badge/fork-painlessMesh-blue)
![library-registry external](https://img.shields.io/badge/external-library--registry-lightgrey)
![EByte LoRa library external](https://img.shields.io/badge/external-EByte_LoRa_E220-orange)

## 📌 Mission (Public Scope)

Alteriom publishes open source resources focused on:

* Automated documentation quality, organization, and continuous improvement
* Repository metadata consistency & compliance patterns
* MQTT topic schema standardization & type-safe integration
* Documentation conversion & normalization utilities
* Issue / template automation and reproducible development practices

## 📂 Public Repositories

Only repositories that are publicly accessible are listed. Forks and upstream third‑party references are noted.

| Repository | Type | Focus | Key Capabilities |
|-----------|------|-------|------------------|
| `alteriom-mqtt-schema` | Alteriom (public) | MQTT schemas & TS types | Versioned MQTT topic schemas, TypeScript validation helpers, integration utilities |
| `repository-metadata-manager` | Alteriom (public) | Repo compliance & health | Topic/tag management, metadata normalization, automation hooks |
| `alteriom-docker-images` | Alteriom (public) | Documentation conversion tooling | Word→Markdown conversion, metadata management, validation scripts |
| `.github` | Alteriom (public) | Org-wide GitHub configuration | Profile README, shared issue templates, shared guidelines |
| `painlessMesh` | Third-party fork | Mesh networking library | Reference fork of release 1.5.6 (no Alteriom modifications) |
| `library-registry` | External upstream | Arduino Library Manager registry | Read-only upstream registry reference |
| `EByte_LoRa_E220_Series_Library` | External upstream | LoRa device library | Multi-platform LoRa E220 LLCC68 reference implementation |

Internal repositories are intentionally not referenced.

## 🔧 Public Tooling Highlights

### Metadata & Compliance

* Repository metadata normalization (topics/tags, descriptions) via `repository-metadata-manager`
* Consistent naming & tagging guidance (see `docs/README.md`)

### Schemas & Validation

* MQTT topic & payload schema versioning (`alteriom-mqtt-schema`)
* TypeScript helpers for compile-time integration safety

### Documentation Conversion

* Word / binary document to Markdown conversion (pandoc scripts in `alteriom-docker-images`)
* Metadata enrichment & standardized front matter

### Configuration & Org Assets

* Shared issue templates and guidelines in `.github`
* Badges maintained for public visibility only

### External References

* Forked mesh networking library (`painlessMesh`) retained for evaluation
* Upstream registries and device libraries (`library-registry`, `EByte_LoRa_E220_Series_Library`)

## 📘 Documentation Standards

Common themes across repositories:

* Kebab-case markdown filenames
* Factual sections only (no performance claims)
* Badges restricted to verifiable public data
* Clear separation of public vs internal scope

## 🚀 Getting Started (Public Repos)

Clone only the public repositories relevant to your work:

```bash
git clone https://github.com/Alteriom/alteriom-mqtt-schema.git
git clone https://github.com/Alteriom/repository-metadata-manager.git
git clone https://github.com/Alteriom/alteriom-docker-images.git
git clone https://github.com/Alteriom/.github.git
git clone https://github.com/Alteriom/painlessMesh.git            # fork
git clone https://github.com/arduino/library-registry.git         # upstream reference
git clone https://github.com/xreef/EByte_LoRa_E220_Series_Library.git
```

### MQTT Schema (`alteriom-mqtt-schema`)

```bash
cd alteriom-mqtt-schema
npm install
npm test   # run validation helper tests (if present)
```

Use exported TypeScript types for integrating MQTT payload validation.

### Repository Metadata Manager (`repository-metadata-manager`)

```bash
cd repository-metadata-manager
npm install
npm run build
npm test   # run compliance/metadata tests (if available)
```

Automates consistent topics, tags, and naming patterns across repositories.

### Documentation Conversion (`alteriom-docker-images`)

```bash
cd alteriom-docker-images
./scripts/convert.sh path/to/input.docx output.md   # example (adjust per repo docs)
```

Refer to repository scripts for pandoc invocation & metadata normalization.

### Mesh Networking (`painlessMesh` fork)

```bash
cd painlessMesh
platformio run
```

Used as reference for internal mesh-related development (no modifications beyond fork metadata).

### LoRa E220 Device Library (external)

```bash
cd EByte_LoRa_E220_Series_Library
platformio run
```

Integrate with ESP32 / ESP8266 builds requiring LoRa E220 support.

## 🧪 Testing & Validation (Public Scope)

* TypeScript schema tests (`alteriom-mqtt-schema`)
* Metadata normalization tests / build validation (`repository-metadata-manager`)
* Conversion script smoke tests (if present) in `alteriom-docker-images`

## 🔐 Security (Public Scope)

* No formal audits or certifications published – do not imply them.
* Recommended: security disclosures via SECURITY.md process.

## 🛠 Contribution Guidelines

Public contributions should:

1. Target only repositories listed in the public table.
2. Avoid referencing internal systems or private code.
3. Include tests for schema or metadata changes.
4. Update documentation front matter consistently.
5. Follow behavior standards (see CODE_OF_CONDUCT.md).

## 📊 Improvement Focus (Public)

* Metadata consistency & tag hygiene
* Schema version clarity & changelog discipline
* Conversion script robustness & reproducibility
* Reduction of unnecessary badges or claims

## 🗺 Public Roadmap Signals

Near-term (public scope):

* Schema versioning enhancements & diff tooling
* Automated metadata normalization checks (workflow)
* Document conversion template improvements

## 📄 Licensing

* This repository: MIT License (see LICENSE)
* Each public repo should include a license file (MIT unless stated otherwise)
* External forks retain original upstream licenses

## 💬 Communication

* Use GitHub Issues and Discussions (where enabled)
* Security concerns: follow SECURITY.md disclosure instructions
* No off-platform support channels listed

## ✅ Verification & Integrity

Public artifacts demonstrate:

* Schema validation & metadata tests
* Documentation conversion examples
* Clear separation of public vs internal scope

## 🤝 How to Help

* Open issues proposing improvements to schema clarity or metadata hygiene
* Contribute conversion script edge cases & test fixtures
* Suggest badge reductions or clarity improvements
* Add missing LICENSE or README files in public repos

---
If you spot inaccurate public information, open an issue titled "Public README Accuracy" with a verifiable source.

_This README lists only publicly observable assets._

---
Maintainer resources: see `docs/README.md` for badge guidelines, update cadence, and workflow plans.

Baseline documents: [`LICENSE`](../LICENSE) | [`CODE_OF_CONDUCT.md`](../CODE_OF_CONDUCT.md) | [`CONTRIBUTING.md`](../CONTRIBUTING.md) | [`SECURITY.md`](../SECURITY.md)
