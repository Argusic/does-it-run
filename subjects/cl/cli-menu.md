# cli-menu

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/php-school/cli-menu, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/cli-menu

## Pinned environment

- Project commit: `342936fabbcb27f8e14f0b695a017b42abfa72a3`
- Test commit: `342936fabbcb27f8e14f0b695a017b42abfa72a3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 5.3 | 3 | 3 | [run](https://argusic.com/run/8d70f766-a585-4153-9a41-4deec0778f42) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PHP not installed in container`
- 1 min: `Minimal PHP build lacks openssl extension, blocking Composer install`
- `stty: 'standard input': Inappropriate ioctl for device (cosmetic TTY warnings)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
