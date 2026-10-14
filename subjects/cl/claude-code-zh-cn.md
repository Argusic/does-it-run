# claude-code-zh-cn

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/taekchef/claude-code-zh-cn, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/claude-code-zh-cn

## Pinned environment

- Project commit: `4dada0ea9524f74e1436a5f968b21e2d609e5847`
- Test commit: `4dada0ea9524f74e1436a5f968b21e2d609e5847`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.8 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.7 | 17.8 | 1 | 1 | [run](https://argusic.com/run/99b7c274-f247-4c3c-94d5-6a566259c9f2) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `4 tests fail because node:sqlite is not available (Node 18.19.1, requires 22.5+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
