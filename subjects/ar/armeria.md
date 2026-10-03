# armeria

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/line/armeria, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/armeria

## Pinned environment

- Project commit: `e118fd45af4e0d25d1b9bde82c9ecd1676bc376a`
- Test commit: `e118fd45af4e0d25d1b9bde82c9ecd1676bc376a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 63.2 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/9af53506-7618-464f-a96b-4e81a44603ff) |
| 2 | pass | 100 | 12 | 63.2 | 3 | 3 | [run](https://argusic.com/run/e6ce53dc-f1bf-49f2-a2ab-2bc5788d17b5) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `No JDK found in environment`
- 3 min: `Error Prone plugin required JDK 21 (class file version 65.0)`
- 2 min: `Error Prone on JDK 21 requires -XDaddTypeAnnotationsToSymbol=true compiler flag`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
