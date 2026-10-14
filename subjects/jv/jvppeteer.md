# jvppeteer

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fanyong920/jvppeteer, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/jvppeteer

## Pinned environment

- Project commit: `f30e6aaaa1a43f8a8bdc61b6648fd331cc12b00a`
- Test commit: `f30e6aaaa1a43f8a8bdc61b6648fd331cc12b00a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 21.1 to 25.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 21.1 | 0 | 0 | [run](https://argusic.com/run/3f9e0ba6-3760-4825-b9d3-0c6bf364656c) |
| 2 | pass | 100 | 24 | 25.5 | 3 | 3 | [run](https://argusic.com/run/2211f816-568b-4dd4-8100-f2f6e2070e03) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `No Java or Maven installed in the container (missing packages: openjdk-17-jdk, maven)`
- 1 min: `Chrome download script called unzip which was not installed and could not be apt-installed (no root)`
- 1 min: `Chrome crashpad handler binary lacked execute permissions after extraction`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
