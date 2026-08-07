# Contributing to Patterson Companies Projects

Thank you for your interest in contributing to Patterson Companies' open-source and internal projects! We welcome contributions from employees, contractors, and community members. Please take a moment to review this guide before opening an issue or submitting a pull request.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Submitting Pull Requests](#submitting-pull-requests)
- [Development Workflow](#development-workflow)
- [Coding Standards](#coding-standards)
- [Commit Messages](#commit-messages)
- [Review Process](#review-process)

## Code of Conduct

All contributors are expected to uphold our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it before participating. We are committed to maintaining a welcoming and respectful environment for everyone.

## Getting Started

1. **Fork or clone** the repository you want to contribute to.
2. **Read the repository's `README.md`** — each project may have specific setup instructions.
3. **Install dependencies** as described in the project documentation.
4. **Create a branch** for your changes (see [Development Workflow](#development-workflow)).

## How to Contribute

### Reporting Bugs

Before submitting a bug report, please:

- Search existing issues to confirm the bug has not already been reported.
- Collect relevant information: steps to reproduce, expected vs. actual behavior, environment details (OS, language/runtime version, etc.).

When filing a bug report, use the **Bug Report** issue template and provide as much detail as possible.

### Suggesting Enhancements

We welcome feature requests and improvement ideas. Before submitting:

- Check the existing issues and project roadmap to avoid duplicates.
- Clearly describe the problem you are trying to solve and why the enhancement would be valuable.

Use the **Feature Request** issue template for new suggestions.

### Submitting Pull Requests

1. Open an issue first for significant changes so the team can discuss the approach before you invest time coding.
2. Keep pull requests focused — one logical change per PR.
3. Include tests that validate your changes.
4. Update documentation (README, inline comments, etc.) as appropriate.
5. Ensure CI checks pass before requesting review.
6. Fill out the pull request template completely.

## Development Workflow

```bash
# 1. Create a feature branch from main (or the default branch)
git checkout -b feature/your-feature-name

# 2. Make your changes and commit them
git add .
git commit -m "feat: short description of your change"

# 3. Push your branch and open a pull request
git push origin feature/your-feature-name
```

Branch naming conventions:

| Type | Pattern | Example |
|---|---|---|
| Feature | `feature/<description>` | `feature/add-oauth-support` |
| Bug fix | `fix/<description>` | `fix/null-pointer-on-login` |
| Documentation | `docs/<description>` | `docs/update-api-reference` |
| Chore / maintenance | `chore/<description>` | `chore/upgrade-dependencies` |

## Coding Standards

Each repository specifies its own language-specific linting and formatting rules. At a minimum:

- Follow the style guides and lint configurations already present in the repository.
- Write self-documenting code; add comments only where the intent is non-obvious.
- Write or update tests for every functional change.
- Do not introduce new dependencies without team discussion.
- Remove dead code and debug statements before opening a PR.

## Commit Messages

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>(<optional scope>): <short summary>

<optional body>

<optional footer(s)>
```

Common types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `ci`.

Examples:

```
feat(auth): add SSO login via SAML 2.0
fix(api): handle empty response body in order service
docs: clarify setup instructions in README
```

## Review Process

- Pull requests require at least **one approving review** from a maintainer before merging.
- Maintainers may request changes — please address feedback promptly.
- Squash-merge is preferred to keep the main branch history clean.
- Large or risky changes may require additional review or a staged rollout.

Thank you for helping make Patterson Companies' software better! 🎉
