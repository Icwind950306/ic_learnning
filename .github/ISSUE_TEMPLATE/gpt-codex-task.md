---
name: GPT -> Codex Task
about: Let ChatGPT write the plan and Codex execute it
title: "[Task] "
labels: ""
assignees: ""
---

## Goal

Describe the user-facing or developer-facing outcome.

## Context

- Relevant pages, commands, files, APIs, or screenshots:
- Current behavior:
- Desired behavior:

## Constraints

- Keep changes scoped to this issue.
- Preserve existing behavior unless explicitly changed below.
- Do not perform unrelated refactors.

## Planner Instructions for ChatGPT Web

Read this repository and this issue. Do not change code. Write a concrete implementation plan as an issue comment using these headings:

```md
## Implementation Plan
1. ...

## Files Likely Affected
- ...

## Edge Cases
- ...

## Verification
- ...

## Risks
- ...
```

## Executor Instructions for Codex

After ChatGPT web has written the plan, read the latest `Implementation Plan` comment and execute it. Keep the change scoped, run the listed verification, and summarize the result.

## Acceptance Criteria

- [ ] ...
- [ ] ...
- [ ] Tests or verification completed.
