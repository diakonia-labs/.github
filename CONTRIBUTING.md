# Contributing to Diakonia-Labs

Thanks for taking the time to contribute! Every thoughtful bug report, documentation improvement, and code change makes this project better.

Repository: [Diakonia-Labs](https://github.com/diakonia-labs).

## Development setup

1. Fork the repository and clone your fork.
2. Install the project's documented prerequisites and dependencies.
3. Create a branch for your change. Follow the instructions below.

## Testing your changes

Run the checks relevant to your change before opening a pull request. Include a regression test when fixing a bug, and describe how you verified your changes.

## Reporting issues

Search existing issues first. For a bug report, include steps to reproduce, expected and actual behavior, and your environment. Discuss substantial changes before starting work.

## Pull requests

Keep pull requests focused on one change. Explain the problem, your approach, and how you tested it. Link any related issues and respond to review feedback constructively.

## Coding conventions: Branches, commits and pull requests

### Branch names
Format: `type/issue-number-short-description`, lowercase, words separated by hyphens.

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

If you are an external contributor, create the branch in your fork.

### Commits and pull request titles
We follow [Conventional Commits](https://www.conventionalcommits.org/):
`type(scope): description`

Scopes: `app`, `desktop`, `core`, `backend`, `specs`, `docs`, `ci`.

Example: `feat(app): add attendance screen`

Every commit must be signed off under the DCO (`git commit -s`). See [Developer Certificate of Origin](#developer-certificate-of-origin-dco).

### Pull requests
- One pull request per issue, as small as possible.
- Link the issue in the description with `Closes #<issue-number>` (for example, `Closes #42`).
- Open a draft pull request if it isn't ready for review yet.
- The title must follow the Conventional Commits format: this is checked automatically.
- Pull requests are merged with *squash merge*: the title becomes the commit message on `main`.
- Nothing is merged without passing checks and approval from a maintainer.

### Developer Certificate of Origin (DCO)
By signing off your commits, you certify that you wrote the code or have the right to submit it under the project's license, as described in the [Developer Certificate of Origin](https://developercertificate.org/).

To sign off, add `-s` when committing:

    git commit -s -m "feat(app): add attendance screen"

This adds a line like this to the commit message:

    Signed-off-by: Your Name <your@email.com>

Pull requests with commits that are not signed off cannot be merged.

## Beyond code

Code is only one way to help. You can improve documentation, reproduce an issue, suggest clearer wording, or help someone get started.

## Security

Do not report vulnerabilities in public issues. Contact [the security team](mailto:diakonia-labs@gmail.com) privately with reproduction details.

## Code of conduct

Please read and follow our [Code of Conduct](https://github.com/diakonia-labs/.github/blob/main/CODE_OF_CONDUCT.md) in all project spaces.
