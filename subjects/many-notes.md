# many-notes

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/brufdev/many-notes, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/many-notes

## Pinned environment

- Project commit: `72ce5bee7a9496c85fbb8ebebca8029718262e1d`
- Test commit: `72ce5bee7a9496c85fbb8ebebca8029718262e1d`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 19.5 to 26.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 19.5 | 3 | 3 | [run](https://argusic.com/run/373d1c45-ba2e-4517-8afd-fb8eda68ddf9) |
| 2 | pass | 100 | 27 | 26.8 | 3 | 3 | [run](https://argusic.com/run/9145921f-c051-4031-8b2a-2838af7ac031) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP 8.4 not installed in container; static binary downloaded from static-php.dev`
- 5 min: `Frontend build fails: Node v18 lacks styleText export needed by rolldown (Vite 8)`
- 5 min: `artisan serve returns empty reply due to Vite manifest not found in production`

Attempt 2:

- 3 min: `No PHP interpreter found on system`
- 2 min: `Node.js v18 too old for Vite 8 (needs styleText export)`
- 3 min: `Composer not available on system`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
