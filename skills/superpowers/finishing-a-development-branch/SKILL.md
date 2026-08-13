---
name: finishing-a-development-branch
description: Complete an authorized commit, push, integration, PR, branch, or worktree action while preserving user state. Use after relevant verification when the user or repository requires delivery.
---

# Finishing a Development Branch

Record initial status, branch, and worktree path before state changes; preserve unrelated work.

Confirm the task diff and fresh delivery checks. Do not require a separate plan, log, or reconciliation artifact unless the user or repository does.

- Perform already-authorized commit or push after verification.
- Ask only when merge, PR, push, retention, or cleanup authority is unresolved.
- Do not switch branches, pull, merge into a base, create a PR, or force-push without authority.
- In detached or host-managed workspaces, name the limitation and preserve work for the host.
- Remove only session-created worktrees with cleanup authority and no required work remaining. First run `git status --short --untracked-files=all --ignored=matching`; if nonempty, list entries. Ignore only verified regenerable artifacts; otherwise ask whether to commit, move, or delete. Never force removal without explicit destructive authorization.

On commit/push failure, preserve verified state and report the error. Do not pull, rebase, merge, or force without separate authority.

Offer discard only when requested. List the branch, unique commits, uncommitted files, and worktree path; require exact affirmative confirmation `discard <target>`.

Report checks, commit/branch state, remote action, and preserved work. Use repository wrappers for shell commands.
