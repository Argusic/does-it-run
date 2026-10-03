# brag

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/latent-spaces/brag, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/brag

## Pinned environment

- Project commit: `c893c5ed52aed84e3e2ee56787de869fccdae6b0`
- Test commit: `c893c5ed52aed84e3e2ee56787de869fccdae6b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.6 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 14.6 | 5 | 5 | [run](https://argusic.com/run/d1a3c207-c427-4e0b-b1b6-76965287823f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 too old for Hyperframes (needs >=22)`
- 2 min: `sharp module failed via npx (glibc/ABI mismatch on cached binary)`
- 2 min: `unzip not available and no root for apt install`
- 3 min: `Hyperframes browser ensure download hung on progress spinner`
- 2 min: `Hyperframes doctor still reported Chrome missing after cache placement`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
