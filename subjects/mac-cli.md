# Mac-CLI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/guarinogabriel/Mac-CLI, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/mac-cli

## Pinned environment

- Project commit: `26c047242351e4b1c66bff91548a07352a694f16`
- Test commit: `26c047242351e4b1c66bff91548a07352a694f16`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.33 | 6.4 | 1 | 1 | [run](https://argusic.com/run/3d310ae2-f18a-4185-9d8b-f211261ddf64) |

## What was observed on a clean machine

Attempt 1:

- 0.08 min: `The shebang was #!/bin/sh but the script uses bash-specific syntax ([[ ]] arrays, etc.), and /bin/sh is dash on this Linux container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
