# ic_learnning

This repository is configured for a GitHub Issue based GPT -> Codex workflow.

## Workflow

1. Create a GitHub issue using the `GPT -> Codex Task` template.
2. Ask ChatGPT on the web to read the repository and write an implementation plan as an issue comment.
3. Ask Codex to read the same issue and execute the plan.
4. Codex should make scoped changes, run verification, and report results back in the issue or PR.

## Standard handoff prompt

Use this prompt in ChatGPT web after opening an issue:

```text
Read this repository and the GitHub issue. Do not change code. Write a concrete implementation plan as an issue comment using these headings: Implementation Plan, Files Likely Affected, Edge Cases, Verification, Risks.
```

Use this prompt in Codex after ChatGPT has written the plan:

```text
Read https://github.com/Icwind950306/ic_learnning/issues/<number>, follow the latest Implementation Plan comment, implement the change, run the listed verification, and summarize what changed.
```
