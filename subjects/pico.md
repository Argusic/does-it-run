# Pico

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/picocms/Pico, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/pico

## Pinned environment

- Project commit: `5e8e0a03f4a14d4f70a109e8f5d905fbbad897f6`
- Test commit: `5e8e0a03f4a14d4f70a109e8f5d905fbbad897f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 45.9 to 45.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 45.9 | 5 | 5 | [run](https://argusic.com/run/bef467eb-c6a9-463f-b3ac-eed350f17d16) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP not installed in container`
- 1 min: `Composer not installed`
- 1 min: `composer install blocked on security advisories for twig/twig and symfony/yaml (old dependencies)`
- 0.5 min: `Missing config/config.yml`
- 1 min: `Default theme uses API version 0 but Pico provides API version 3 and PicoDeprecated isn't available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
