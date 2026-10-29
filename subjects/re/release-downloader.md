# release-downloader

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/robinraju/release-downloader, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/release-downloader

## Pinned environment

- Project commit: `64affece560bf7e81ec9e2489777b5ab65a8ff5a`
- Test commit: `64affece560bf7e81ec9e2489777b5ab65a8ff5a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 3.2 | 1 | 1 | [run](https://argusic.com/run/05ced52c-4bff-4377-950a-8bbd9092d9bb) |

## What was observed on a clean machine

Attempt 1:

- `Engine requirement mismatch: package.json requires node >=24.0.0, system has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
