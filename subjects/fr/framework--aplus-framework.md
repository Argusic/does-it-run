# framework

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aplus-framework/framework, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/run/d57c5cb8-f9f5-48d0-abba-e02f04501c59

## Pinned environment

- Project commit: `22e6cff5fe3fcf2958e9e6108b3439ec568038dd`
- Test commit: `22e6cff5fe3fcf2958e9e6108b3439ec568038dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.6 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.6 | 2 | 2 | [run](https://argusic.com/run/d57c5cb8-f9f5-48d0-abba-e02f04501c59) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP and Composer not pre-installed in container`
- 2 min: `Missing PHP extensions: ext-xdebug, ext-sodium, ext-intl, ext-memcached required by composer.json dependencies`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
