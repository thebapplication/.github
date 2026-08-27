# Contributing

These guidelines apply to every repository in the WeAreB organisation.

## Prerequisites

- Read the repository `README.md` for stack-specific setup.
- Request access to the relevant repository and environments before starting.
- Confirm you can run the project and its test suite locally.

## Branches

- Base all work on `main`.
- Branch names use the format `type/short-description`, for example
  `feat/court-availability-filter` or `fix/booking-timezone`.
- Keep branches short-lived. Rebase on `main` rather than merging it back in.

## Commits

- Follow [Conventional Commits](https://www.conventionalcommits.org).
- Allowed types: `feat`, `fix`, `perf`, `refactor`, `docs`, `test`, `build`,
  `ci`, `chore`, `revert`.
- Commitlint and Husky run on commit. Do not bypass hooks with `--no-verify`.
- Write commit messages in the imperative mood and explain the reason for the
  change in the body when it is not obvious.

## Pull requests

- One logical change per pull request. Split unrelated work.
- Fill in the pull request template in full.
- Link the issue the work resolves.
- Ensure CI passes. Pull requests with failing checks are not reviewed.
- At least one approving review from a code owner is required to merge.
- Resolve all review threads before merging.
- Use squash merge. The squash title must be a valid Conventional Commit.

## Code quality

- Run the formatter and linter before pushing. Both are enforced in CI.
- Add or update tests for every behavioural change.
- Update documentation, environment examples, and changelogs affected by the
  change.
- Do not commit secrets, credentials, or generated build output.

## Reviews

- Review within one working day where possible.
- Comment on the change, not the author.
- Approve only when the change is correct, tested, and understood.

## Reporting problems

- Bugs and feature requests: open an issue using the appropriate form.
- Security vulnerabilities: follow [SECURITY.md](SECURITY.md). Do not open a
  public issue.
