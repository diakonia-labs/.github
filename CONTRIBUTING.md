# Contributing to Diakonia Labs

Thanks for taking the time to contribute! Every thoughtful bug report, documentation improvement, and code change makes this project better.

Organization: [Diakonia Labs](https://github.com/diakonia-labs)

## Table of contents

- [Code of conduct](#code-of-conduct)
- [Security](#security)
- [Ways to contribute](#ways-to-contribute)
- [Reporting issues](#reporting-issues)
  - [Issue titles](#issue-titles)
- [Development setup](#development-setup)
- [Testing your changes](#testing-your-changes)
- [Branch names](#branch-names)
- [Commit messages](#commit-messages)
- [Pull requests](#pull-requests)
  - [Pull request titles](#pull-request-titles)
  - [Pull request rules](#pull-request-rules)
- [Developer Certificate of Origin (DCO)](#developer-certificate-of-origin-dco)

## Code of conduct

Please read and follow our [Code of Conduct](https://github.com/diakonia-labs/.github/blob/main/CODE_OF_CONDUCT.md) in all project spaces.

## Security

Do not report vulnerabilities in public issues. Contact [the security team](mailto:diakonia-labs@gmail.com) privately with reproduction details.

## Ways to contribute

Code is only one way to help. You can also:

- Report a bug or reproduce an existing one.
- Improve the documentation or suggest clearer wording.
- Propose an improvement or a new feature.
- Help someone get started.

## Reporting issues

Search existing issues first. Discuss substantial changes before starting work. For questions, use Discussions instead of issues.

For a bug report, include steps to reproduce, expected and actual behavior, and your environment.

### Issue titles

Format: `[Type] Short description`

Issue titles are checked automatically. If the format is wrong, you will get a comment explaining how to fix it, and the `needs-title-fix` label will be added until you edit the title.

| Type | Use | Example |
|---|---|---|
| `[Bug]` | Something doesn't work as expected | `[Bug] Members are duplicated after syncing` |
| `[Feature]` | A new feature | `[Feature] Record attendance with a QR code` |
| `[Improvement]` | An improvement to an existing feature | `[Improvement] Sort the members list by last name` |
| `[Docs]` | Documentation | `[Docs] Add a self-hosting guide` |
| `[Spec]` | A new spec or a change to an existing spec | `[Spec] Define roles and permissions for v1` |

## Development setup

1. Fork the repository and clone your fork.
2. Install the prerequisites and dependencies described in the repository's README.
3. Create a branch for your change, following the [branch naming rules](#branch-names).

## Testing your changes

Run the checks relevant to your change before opening a pull request. Include a regression test when fixing a bug, and describe how you verified your changes.

## Branch names

Format: `type/issue-number-short-description`, lowercase, words separated by hyphens.

If you are an external contributor, create the branch in your fork.

| Type | Use | Example |
|---|---|---|
| `feat/` | New feature | `feat/42-qr-invitations` |
| `fix/` | Bug fix | `fix/57-sync-duplicates-members` |
| `docs/` | Documentation | `docs/12-installation-guide` |
| `spec/` | New specs or changes to specs | `spec/30-roles-and-permissions` |
| `refactor/` | Internal changes that don't alter behavior | `refactor/61-core-queries` |
| `test/` | Tests | `test/44-invitation-tests` |
| `chore/` | Maintenance and dependencies | `chore/70-update-expo` |
| `ci/` | Continuous integration and automation | `ci/15-macos-signing` |
| `hotfix/` | Urgent fixes on a released version | `hotfix/88-crash-on-startup` |

## Commit messages

We follow [Conventional Commits](https://www.conventionalcommits.org/), with the same format as [pull request titles](#pull-request-titles):

    feat(app): add attendance screen

Every commit must be signed off under the [DCO](#developer-certificate-of-origin-dco) (`git commit -s`).

## Pull requests

### Pull request titles

Format: `type(scope): description`

Pull request titles are checked automatically, and a pull request can't be merged until its title is valid. Because we use squash merge, the title becomes the commit message on `main`.

**Types**

| Type | Use | Example |
|---|---|---|
| `feat` | New feature | `feat(app): add attendance screen` |
| `fix` | Bug fix (also for hotfixes) | `fix(core): prevent duplicate members after syncing` |
| `docs` | Documentation | `docs: add installation guide` |
| `spec` | New specs or changes to specs | `spec(specs): define roles and permissions` |
| `refactor` | Internal changes that don't alter behavior | `refactor(core): simplify member queries` |
| `test` | Tests | `test(core): add invitation tests` |
| `chore` | Maintenance and dependencies | `chore(deps): update expo` |
| `ci` | Continuous integration and automation | `ci: sign macOS builds` |
| `perf` | Performance improvements | `perf(app): speed up the members list` |

**Scopes (optional)**

| Scope | Part of the project |
|---|---|
| `app` | The app: screens and components (mobile, tablet and desktop) |
| `desktop` | The Electron desktop shell |
| `core` | Shared logic: data, queries, validation and permissions |
| `backend` | The server |
| `specs` | Specs and the project constitution |
| `docs` | Documentation |
| `ci` | Continuous integration and automation |
| `deps` | Dependencies |

**Writing the description**

- Use the imperative mood: `add`, `fix`, `update` (not `added` or `adds`).
- Start in lowercase and don't end with a period.
- Keep the whole title under 72 characters.
- Add `!` after the type or scope for breaking changes: `feat(core)!: change the member data format`.

### Pull request rules

- One pull request per issue, as small as possible.
- Explain the problem, your approach, and how you tested it.
- Link the issue in the description with `Closes #<issue-number>` (for example, `Closes #42`). The issue will close automatically when the pull request is merged.
- Open a draft pull request if it isn't ready for review yet.
- Respond to review feedback constructively.
- Nothing is merged without passing checks and approval from a maintainer.

## Developer Certificate of Origin (DCO)

By signing off your commits, you certify that you wrote the code or have the right to submit it under the project's license, as described in the [Developer Certificate of Origin](https://developercertificate.org/).

To sign off, add `-s` when committing:

    git commit -s -m "feat(app): add attendance screen"

This adds a line like this to the commit message:

    Signed-off-by: Your Name <your@email.com>

Pull requests with commits that are not signed off cannot be merged.
