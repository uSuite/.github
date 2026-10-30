# Contributing to uSuite

Thank you for looking. Every repository here is small and kept by one person, so a short issue that says what you did, what you expected and what happened, with the macOS version and the tool's version (`make version`, or the About box), goes a long way.

Pull requests are welcome for fixes and for items already in a repository's `docs/01-backlog.md`. For anything larger, open an issue first, so we can agree on it before you spend the time; each repository's `docs/DECISIONS.md` says what is in scope and why.

How the repositories work:

- Branches follow git-flow: work on `feature/<name>` off `develop`, and pull requests target `develop`. `master` only moves on a release.
- `make test` passes before every commit; for the apps, `make app` and `make smoke` pass before a change to the interface.
- One logical change per commit, and the message says why.
- No third-party packages; the tools use Apple frameworks only.
- Shared code changes in scommon first, with tests, then the tools raise their minimum version.
- Docs are plain text, one paragraph per line.

By contributing you agree that your work is released under the repository's MIT licence.
