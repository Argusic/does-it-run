# mindroom

**Verdict: not yet verified.** Not scored (no completed run has a score).

Project: https://github.com/mindroom-ai/mindroom, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mindroom

## Pinned environment

- Project commit: `fea2b810ecaac6e9e07695076e60d30a4d15e82c`
- Test commit: `fea2b810ecaac6e9e07695076e60d30a4d15e82c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 89.8 to 89.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 0.5 | 89.8 | 1 | 1 | [run](https://argusic.com/run/d415979d-691b-4fbf-be90-2698f75ef64c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `2 CLI tests failed due to Rich soft-wrapping stripping spaces between words in console output, causing substring assertions to fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
