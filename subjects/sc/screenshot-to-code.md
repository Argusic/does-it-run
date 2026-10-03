# screenshot-to-code

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/abi/screenshot-to-code, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/screenshot-to-code

## Pinned environment

- Project commit: `d026163f586dfa8c5c10d28c36edd59a9d3b0e88`
- Test commit: `d026163f586dfa8c5c10d28c36edd59a9d3b0e88`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 5.6 to 23.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 16.8 | 2 | 2 | [run](https://argusic.com/run/1934e9c4-d25d-45d0-b47e-967f3a709821) |
| 2 | pass | 100 | 5 | 5.6 | 0 | 0 | [run](https://argusic.com/run/29cbc9ac-5167-48cb-97d4-08ee8460570f) |
| 3 | pass with mocks | 92 | 22.7 | 23.2 | 4 | 4 | [run](https://argusic.com/run/01285aad-9c4a-4835-9ff1-c858cec5444c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Python externally-managed environment blocks pip install of poetry`
- 3 min: `pnpm v11 requires Node >=22, but Node 18 is available`

Attempt 3:

- 2 min: `poetry not found in PATH`
- 1 min: `pnpm not found in PATH`
- 1 min: `pip3 install --user poetry blocked by PEP 668`
- 1 min: `npm install -g pnpm blocked by permissions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
