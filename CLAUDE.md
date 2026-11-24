# Repository rules for Claude sessions

Several Claude Code sessions work in this repository at the same time, each on its own
`claude/*` branch, and some sessions start from `main`.

- Never delete `main`, and never change the repository's default branch.
- Never delete, force-push or rewrite another session's `claude/*` branch.
- When merging a pull request, do not use "delete branch" on `main` or on a branch another
  session still uses.
- Ask the user before any repository setting change (branch deletion, default branch,
  branch protection, force push).
- Start new sessions from the working branch they continue (`source_revision`), not from
  `main`, so a missing `main` cannot block them.
- Never commit private files (photos of the child, passports, bank statements, visa
  documents). Keep them in the scratchpad or the user's Google Drive.
