# aurelio-finance

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LosaLosSantos/aurelio-finance, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/aurelio-finance

## Pinned environment

- Project commit: `49ac69a4ffbd8e084bd3aea62762991a1897051a`
- Test commit: `49ac69a4ffbd8e084bd3aea62762991a1897051a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.5 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 4.5 | 0 | 0 | [run](https://argusic.com/run/3306f93a-f30a-40f0-b2b8-8e0baad52ee0) |
| 2 | pass | 100 | 6 | 4.7 | 3 | 3 | [run](https://argusic.com/run/63d97e65-0a92-4496-b9d4-d305d49c5f6a) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `uv not found on PATH`
- 2 min: `Node.js v18 too old for build toolchain (needs v22+)`
- 1 min: `rolldown native binding @rolldown/binding-linux-x64-gnu missing after npm install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
