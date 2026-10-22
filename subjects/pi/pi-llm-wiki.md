# pi-llm-wiki

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zosmaai/pi-llm-wiki, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-llm-wiki

## Pinned environment

- Project commit: `f0b6959be399a43b816bc8e6871a6ebcb6cf2ea6`
- Test commit: `f0b6959be399a43b816bc8e6871a6ebcb6cf2ea6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.9 | 1 | 1 | [run](https://argusic.com/run/9ed468f8-523e-49f6-bd5c-2308245722b9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container Node is v18.19.1 but package.json engines requires >=22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
