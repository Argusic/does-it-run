# drawthe.net

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cidrblock/drawthe.net, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/drawthe-net

## Pinned environment

- Project commit: `c71cdba4c3bdb53e4a2310f8636aa6c1ad73f4ae`
- Test commit: `c71cdba4c3bdb53e4a2310f8636aa6c1ad73f4ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 7.6 | 1 | 1 | [run](https://argusic.com/run/9e2c9107-b334-4442-894e-3792c66a281a) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `CLI renderer crashed in d3-zoom: ReferenceError: navigator is not defined (node 18/jsdom headless render)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
