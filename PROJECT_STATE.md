# Project state

Updated: 2026-08-28 (Europe/Moscow)

## Identity

- Project: `ipatool-sapfix`, macOS App Store authentication compatibility fork.
- Canonical local root: `~/Projects/active/ipatool-sapfix`.
- Compatibility path: the former local Codex root points to the canonical root.
- Public repository: `https://github.com/maksimryabkin/ipatool-sapfix.git`.
- Branch: `main`.
- Verified source snapshot: `6fb420d04ef884515dd4ddf7f676b5cfe6af3252`.
- Current release: `2.3.2-sapfix.1`.
- The current local issue-monitoring task is retained.

## Verification

- Local `main` and live `origin/main` were equal at the verified snapshot.
- `go test ./...`: passed on 2026-08-28.
- `go build ./...`: passed on 2026-08-28.
- Matching pre/post move manifests cover 220 files, 75 directories, and
  3,046,658 file bytes.
- A complete verified bundle preserves all local branches, remotes, tags, and
  Codex turn-diff checkpoint refs.

## Product state

- Fresh interactive login and an authenticated version-list request were
  reported successful on Apple Silicon/macOS on 2026-08-28.
- The repository is public and currently receives support traffic.
- Issue #1 remains open as a potentially environment-dependent authentication
  bug; issue #3 remains open as a support question. Issues #2 and #4 are closed.
- A downstream repository copied the Git history and continued independently.
  It is not a GitHub-native fork, but it preserves history and the MIT license.
  Do not import its session-transfer or GitHub Actions changes without a
  separate security review.

## Security and local state

- Apple account identity, password, two-factor codes, DSID, cookies, and session
  tokens must never be committed, pasted into issue comments, or recorded in
  this state file.
- Local authentication state belongs to macOS Keychain and is not part of this
  repository or its backup.
- Keep tests and issue responses redacted. Avoid verbose authentication logs in
  public reports.

## Next actions

1. Monitor open issues and wait for affected users to confirm whether the
   post-August-27 login failures persist.
2. Reproduce any new authentication report without publishing account data.
3. Keep future Codex work rooted at the canonical path.
4. Retain the current ipatool task while public issue monitoring is active.

The unrelated BotHelp/MAX attribution task that happened to use the old ipatool
working directory is not part of this product and must not be merged into its
source or continuity.
