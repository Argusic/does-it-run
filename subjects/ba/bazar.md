# bazar

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/conedevelopment/bazar, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/bazar

## Pinned environment

- Project commit: `32bc97a593915ca40e1323239b6ffd9582aa2f5f`
- Test commit: `32bc97a593915ca40e1323239b6ffd9582aa2f5f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 6 | 2 | 2 | [run](https://argusic.com/run/454a4b9f-6565-41b5-8407-7a42f31e8d08) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No PHP or Composer present and no root to apt-install; installed self-contained toolchain (micromamba + conda-forge PHP 8.5.9, Composer phar) under /tmp`
- 6 min: `conedevelopment/root requires ext-gd which the conda-forge PHP build lacks; composer install failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
