# product-microgateway

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wso2/product-microgateway, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/product-microgateway

## Pinned environment

- Project commit: `7f01aaeae542c8f659a81b6bb506688c1651c806`
- Test commit: `7f01aaeae542c8f659a81b6bb506688c1651c806`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.5 to 24.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 24.5 | 4 | 4 | [run](https://argusic.com/run/2eb218ca-3e30-49fd-885f-6a63eda5c01b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `JDK 11 not available in container`
- 2 min: `Maven not available in container`
- 5 min: `Go (golang.org) not available in container`
- 5 min: `Missing config.toml/log_config.toml for adapter tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
