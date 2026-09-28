# Contributing to Alteriom projects

Thanks for taking the time to contribute. This guide applies to every public Alteriom repository
that doesn't have its own `CONTRIBUTING.md`. If the repository you're working in has one, follow
that instead.

## Ways to contribute

- **Report a bug.** Open an issue with the steps to reproduce it, what you expected and what
  happened. For firmware, include the board, core version and serial output.
- **Suggest an improvement.** Open an issue describing the problem you're trying to solve before
  proposing a solution.
- **Improve the documentation.** Fixes to READMEs, examples and guides are always welcome.
- **Submit code.** Bug fixes and features, with tests where the repository has them.

Security vulnerabilities are the exception: please **don't** open a public issue. Follow the
[security policy](SECURITY.md) instead.

## Before you start

1. Search the existing issues and pull requests; someone may already be on it.
2. For anything larger than a small fix, open an issue first so we can agree on the approach before
   you invest the time.
3. Read the repository's README. Most repositories document how to build and test them there.

## Making a change

1. Fork the repository and create a branch from `main`.
2. Keep the change focused: one fix or feature per pull request.
3. Add or update tests for the behaviour you changed.
4. Update the documentation and the changelog if the repository keeps one.
5. Make sure the build and tests pass locally.
6. Open a pull request and fill in the template.

### Commit messages

Write commit messages in the imperative mood and explain *why* as well as *what*. Many of our
repositories use [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`,
`docs:` and so on) to generate release notes; follow the style you see in the repository's history.

### Firmware and embedded changes

- Say which boards and framework versions you tested on (for example *ESP32-S3, Arduino core
  3.0.x*).
- Keep memory and flash usage in mind on ESP8266 and small ESP32 variants.
- Don't break the public API or wire format without discussing it first. Other projects depend on
  both.

## Review

A maintainer will review your pull request, usually within a week. We may ask for changes; that's a
normal part of the process. Once CI passes and the review is approved, a maintainer merges it.

## Licensing

By contributing, you agree that your contribution is licensed under the license of the repository
you're contributing to (see its `LICENSE` file).

## Code of conduct

Everyone taking part in Alteriom projects is expected to follow our
[code of conduct](CODE_OF_CONDUCT.md).
