# CharDesk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Sayhi-bzb/CharDesk, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/chardesk

## Pinned environment

- Project commit: `bcd0ac864bf27d25a0fc4aab7ba1bc5e75bfd4af`
- Test commit: `bcd0ac864bf27d25a0fc4aab7ba1bc5e75bfd4af`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/cc03d0c0-df4e-45c5-8531-adac63d3d0ce) |
| 2 | pass | 100 | 2 | 6 | 1 | 1 | [run](https://argusic.com/run/2cc57ef4-16b9-4a06-a267-e6ce1f05e8aa) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18.19.1 too old , project requires >=20`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
