# crawler

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spatie/crawler, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/crawler

## Pinned environment

- Project commit: `06c4ddc4839494bb6b872ff550f7828a129c7eef`
- Test commit: `06c4ddc4839494bb6b872ff550f7828a129c7eef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 6.1 | 3 | 3 | [run](https://argusic.com/run/29db566f-ce6e-4ae7-ab4b-43b379cc4d8e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP 8.4 not found in container`
- 0.5 min: `Composer not found in container`
- 1 min: `TestServer.php hardcodes 'php -S' but php not in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
