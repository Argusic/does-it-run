# lineage-skill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JuneYaooo/lineage-skill, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/lineage-skill

## Pinned environment

- Project commit: `7e2cbc5dc317139f39c86f47c60aba4e34ac7838`
- Test commit: `7e2cbc5dc317139f39c86f47c60aba4e34ac7838`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 4.2 | 3 | 3 | [run](https://argusic.com/run/cfe984a6-5dbc-4fbf-926d-2704feabbe9c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `install_as_skill.sh failed with "rsync: command not found" on this container`
- 3 min: `installer copied the skill dir into itself, producing a nested lineage-skill/lineage-skill tree`
- 1 min: `installer pip step failed with PEP 668 externally-managed-environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
