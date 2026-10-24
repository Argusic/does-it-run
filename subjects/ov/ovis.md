# ovis

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/devswha/ovis, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ovis

## Pinned environment

- Project commit: `5253f3bf17fbc96da01e89184afcc47a28b689f6`
- Test commit: `5253f3bf17fbc96da01e89184afcc47a28b689f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 4.1 | 3 | 3 | [run](https://argusic.com/run/5d17e711-05e5-4f80-9778-e1a792dcc5a7) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `Bun not found in container`
- `herdr not installed - the app is a bridge and requires herdr 0.9.0+`
- 0.2 min: `unzip not available for Bun install script`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
