# carapace-bin

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/carapace-sh/carapace-bin, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/carapace-bin

## Pinned environment

- Project commit: `c9cac841afb9ac0265ef7b35b47194756b160d8f`
- Test commit: `c9cac841afb9ac0265ef7b35b47194756b160d8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 12.4 | 2 | 2 | [run](https://argusic.com/run/b0b401ed-c05a-4528-a971-a36db8000fe0) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go (golang) compiler not installed in container`
- 1 min: `NO_COLOR=1 env var caused 4 test failures (style fields stripped from output)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
