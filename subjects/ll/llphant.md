# LLPhant

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LLPhant/LLPhant, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/llphant

## Pinned environment

- Project commit: `d85d902e91ee7a02552bab7a980cf36601be0029`
- Test commit: `d85d902e91ee7a02552bab7a980cf36601be0029`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.5 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 6.3 | 2 | 2 | [run](https://argusic.com/run/890d74b8-79dd-47bd-8e2e-c0266be43244) |
| 2 | pass | 100 | 2.5 | 4.5 | 4 | 4 | [run](https://argusic.com/run/9ce69c9c-4af6-45dc-bbcd-58ea90f9de1a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No PHP interpreter or Composer installed on host`
- 1 min: `ext-mongodb not available in static PHP build, blocking composer install`

Attempt 2:

- 0.5 min: `PHP not installed in container`
- 0.2 min: `ext-mongodb not available in static PHP build`
- 0.1 min: `ext-gd not available in static PHP build`
- 1 min: `Tiktoken vocab download from Azure blob store fails with IOError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
