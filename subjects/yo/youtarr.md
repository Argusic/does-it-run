# Youtarr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DialmasterOrg/Youtarr, licensed ISC, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/youtarr

## Pinned environment

- Project commit: `46c17018fb50ce77369d1f023467587a5db81460`
- Test commit: `46c17018fb50ce77369d1f023467587a5db81460`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.8 to 18.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 18.5 | 4 | 4 | [run](https://argusic.com/run/7240db6d-2a8f-4743-aacc-5e59efdb462e) |
| 2 | pass | 100 | 11 | 14.8 | 6 | 6 | [run](https://argusic.com/run/1b241ef7-3b14-4d3f-a81c-c3755ad9bb5b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `System Node.js v18.19.1 does not meet package.json requirement of >=20.19.0`
- 2 min: `System npm v9.2.0 does not meet package.json requirement of >=11.10.0`
- 3 min: `npm engine check initially failed against eslint-visitor-keys which required ^22.13.0`
- 1 min: `PATH did not include the new Node installation`

Attempt 2:

- 2 min: `Node.js version 18.19.1 does not meet minimum requirement >=20.19.0`
- 1 min: `npm version 9.2.0 does not meet minimum requirement >=11.10.0 for engine-strict`
- 1 min: `Docker is not available`
- 1 min: `MariaDB 10.11.7 binary needs libncurses.so.5 which is not available`
- 3 min: `Mariadb (--skip-grant-tables) crashed on startup`
- `yt-dlp not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
