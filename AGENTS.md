# Repository Instructions for Codex

## Collaboration Model

This repository uses GitHub issues as the handoff surface between ChatGPT web and Codex.

- ChatGPT web is the planner: it should inspect context and write an implementation plan in the issue.
- Codex is the executor: it should read the issue and the latest plan comment, implement the change, verify it, and summarize the result.

## Execution Rules

- Keep changes scoped to the issue goal and acceptance criteria.
- Prefer existing project patterns over new abstractions.
- Do not rewrite unrelated files or perform broad refactors unless the issue explicitly asks for it.
- Preserve user changes already present in the worktree.
- Add or update focused tests when behavior changes.
- Run the verification commands listed in the issue plan when available.
- If verification cannot run, explain why and provide the most relevant fallback checks.

## Expected Codex Summary

When finishing a task, report:

- What changed.
- Files touched.
- Verification commands run and their results.
- Any remaining risks or follow-up work.
