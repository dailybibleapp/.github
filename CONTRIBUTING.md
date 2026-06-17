# Contributing Guide

Thanks for your interest in contributing! This guide applies across all
repositories in the organization unless a repository overrides it with its own.

## Before you start

- Read our [Code of Conduct](CODE_OF_CONDUCT.md).
- Check existing issues and pull requests to avoid duplicates.
- For larger changes, open an issue first to discuss the approach.

## ⚠️ Sensitive data

This and most of our repositories are **public**. Never commit:

- Credentials, API keys, tokens, or private keys
- Personal data (names, emails, phone numbers, addresses, IDs, payment data)
- Internal URLs, infrastructure details, or customer data

Use environment variables or a secrets manager for configuration, and
synthetic placeholders in examples and tests. If you accidentally commit a
secret, rotate it immediately and notify the maintainers.

## Workflow

1. **Fork / branch** — create a feature branch off the default branch.
   - Suggested naming: `feat/<short-description>`, `fix/<short-description>`,
     `docs/<short-description>`, `chore/<short-description>`.
2. **Make focused changes** — keep pull requests small and single-purpose.
3. **Follow existing conventions** — match the code style already present in
   the repository you're working in.
4. **Write tests** — add or update tests for the behavior you change.
5. **Run checks locally** — ensure the build, tests, and linters pass.
6. **Open a pull request** — fill in the
   [pull request template](PULL_REQUEST_TEMPLATE.md) completely.

## Commit messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<optional scope>): <short summary>
```

Common types: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`, `perf`, `ci`.

Example: `fix(auth): reject expired tokens on refresh`

## Pull request expectations

- The PR description explains **what** changed and **why**.
- CI is green (build, tests, linters, security checks).
- Security- and privacy-relevant changes are called out for reviewer attention.
- At least one maintainer approval before merge.

## Code review

Reviews focus on correctness, maintainability, security, performance, and
clarity. Be constructive, assume good intent, and keep feedback technical.

## Questions

See [SUPPORT.md](SUPPORT.md) for where to ask questions.
