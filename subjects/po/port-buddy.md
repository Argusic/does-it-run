# port-buddy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amak-tech/port-buddy, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/port-buddy

## Pinned environment

- Project commit: `59a2ef2b452ffabb32b6914f50860e8cb6523648`
- Test commit: `59a2ef2b452ffabb32b6914f50860e8cb6523648`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.4 | 2 | 2 | [run](https://argusic.com/run/f0c4e45f-b1f9-43e3-af88-ad6f734094e4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Java 25 JDK not found in container`
- 1 min: `Web (npm) build failed: 'URI malformed' on index.html because VITE_CANONICAL env var was unset, leaving %VITE_CANONICAL% literal in HTML`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
