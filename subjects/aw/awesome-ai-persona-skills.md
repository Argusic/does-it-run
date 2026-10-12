# awesome-ai-persona-skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/momozi1996/awesome-ai-persona-skills, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/awesome-ai-persona-skills

## Pinned environment

- Project commit: `729ff734f5edcbaed70e256d1031fd0a224f6527`
- Test commit: `729ff734f5edcbaed70e256d1031fd0a224f6527`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 1.1 to 1.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.17 | 1.1 | 2 | 2 | [run](https://argusic.com/run/99f548ba-b956-4267-bc73-ec3693417b21) |

## What was observed on a clean machine

Attempt 1:

- 0.02 min: `install.sh and tianya-gods scripts in tianya-gods-framework not executable`
- 0.02 min: `DirectorAgents-1 shell scripts not executable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
