# scroll-craft

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nateherkai/scroll-craft, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/scroll-craft

## Pinned environment

- Project commit: `75d81f74e83692add18cd7a8a8e078b8a887a579`
- Test commit: `75d81f74e83692add18cd7a8a8e078b8a887a579`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.8 to 12.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 12.8 | 2 | 2 | [run](https://argusic.com/run/a9680a78-0f19-47f4-aa54-906e02c00b24) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `playwright-core@1.64.1 requires Node >=20 but container has Node 18.19.1, causing EBADENGINE warnings`
- 1 min: `Chrome not found on PATH or standard locations by doctor.mjs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
