# no-ai-slop

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/petergyang/no-ai-slop, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/no-ai-slop

## Pinned environment

- Project commit: `000650b156983f5159695b441477f4e63b25dc85`
- Test commit: `000650b156983f5159695b441477f4e63b25dc85`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 2.2 | 1 | 1 | [run](https://argusic.com/run/ccc982f3-f41f-466c-99fa-77cc4884fb6a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npx skills@1.7.0 requires Node >=22.20.0, container has Node 18.19.1. SyntaxError on styleText export from node:util.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
