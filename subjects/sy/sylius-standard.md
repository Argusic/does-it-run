# Sylius-Standard

**Verdict: runs.** Argusic Score 97.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Sylius/Sylius-Standard, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/sylius-standard

## Pinned environment

- Project commit: `6b580309567f2cf9b840e98efca2c7e3544a55bd`
- Test commit: `6b580309567f2cf9b840e98efca2c7e3544a55bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.2 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 97.14 | 9.5 | 14.2 | 7 | 6 | [run](https://argusic.com/run/dc499d92-4213-49fb-91cd-f3253a2084eb) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `PHP not found in container`
- 0.5 min: `Composer not found`
- 1.5 min: `FOSRestBundle class not found , friendsofsymfony/rest-bundle missing from dependencies`
- 0.5 min: `PHP memory limit exhaustion (128M default)`
- 2 min: `MySQL connection refused , no MySQL server available`
- 1.5 min: `Webpack entrypoints.json missing , frontend build incomplete`
- 1 min: `npm install failed , Node.js v18 does not meet Sylius requirement Node.js ^22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
