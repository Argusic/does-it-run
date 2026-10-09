# openspout

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openspout/openspout, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/openspout

## Pinned environment

- Project commit: `f6a027ad119abe7c1986cee397bae0694e2af4bd`
- Test commit: `f6a027ad119abe7c1986cee397bae0694e2af4bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.1 to 20.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 20.1 | 4 | 4 | [run](https://argusic.com/run/6ba9d62e-b123-456a-ba27-ebd7298cf3d0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP and Composer not pre-installed`
- 1 min: `Static PHP warns extensions can't be dynamically loaded`
- 1 min: `phpunit.xml failOnAllIssues=true blocks tests due to coverage warning`
- 2 min: `libxml 2.12.5 max amplification check breaks quadratic blowup test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
