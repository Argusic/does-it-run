# NoteDiscovery

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gamosoft/NoteDiscovery, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/notediscovery

## Pinned environment

- Project commit: `4e2a027a989e2353282ecccb920098f81e9e843e`
- Test commit: `4e2a027a989e2353282ecccb920098f81e9e843e`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.9 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 3 | 8.3 | 2 | 2 | [run](https://argusic.com/run/6d79300e-8a04-439f-95a2-e0fded691d4e) |
| 2 | pass | 100 | 0.5 | 4.9 | 0 | 0 | [run](https://argusic.com/run/a083a556-2a61-42de-a176-b94fca9d5099) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pip not found in container (no ensurepip, no python3-venv, cannot apt), requiring bootstrap via get-pip.py with --break-system-packages`
- 1 min: `All 20 frontend vendor browser libraries missing on first startup - web UI would not load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
