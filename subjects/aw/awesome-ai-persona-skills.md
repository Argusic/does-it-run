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
- Valid runs: 2; wall time 1.1 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.17 | 1.1 | 2 | 2 | [run](https://argusic.com/run/99f548ba-b956-4267-bc73-ec3693417b21) |
| 2 | pass with mocks | 92 | 4 | 4.6 | 4 | 4 | [run](https://argusic.com/run/99687201-3a3f-473f-8bea-82ba50dce77e) |

## What was observed on a clean machine

Attempt 1:

- 0.02 min: `install.sh and tianya-gods scripts in tianya-gods-framework not executable`
- 0.02 min: `DirectorAgents-1 shell scripts not executable`

Attempt 2:

- 1 min: `Missing execute permissions on shell scripts (test.sh, install.sh, tianya-gods)`
- 1 min: `Python module name mismatch: scripts/team-orchestrator.py (hyphen) vs __init__.py importing team_orchestrator (underscore) caused ImportError`
- 1 min: `Installed tianya-gods CLI script used BASH_SOURCE[0] without readlink, breaking when invoked via symlink at ~/.local/bin/`
- 0.5 min: `~/.local/bin/ directory did not exist, so install.sh symlink failed silently`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
