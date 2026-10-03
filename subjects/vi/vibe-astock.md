# vibe-astock

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/simonlin1212/vibe-astock, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/vibe-astock

## Pinned environment

- Project commit: `d7a0e568424f5c0b1de9e39b1ddd733ecdbf9edb`
- Test commit: `d7a0e568424f5c0b1de9e39b1ddd733ecdbf9edb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 11.2 to 21.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 21.7 | 2 | 2 | [run](https://argusic.com/run/5e828a96-83ea-47c8-8c4e-96cc6da07cf5) |
| 2 | pass with mocks | 92 | 3 | 11.2 | 2 | 2 | [run](https://argusic.com/run/ac7e0c79-109d-450f-a017-a2aff052c3f5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `socket._fallback_socketpair() removed in Python 3.12`
- 3 min: `bridge main.mjs imports .ts without a TypeScript loader`

Attempt 2:

- 2 min: `System Node.js 18.19.1 is below required v22+`
- 1 min: `test_core_logic.py references socket._fallback_socketpair() removed in Python 3.12`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
