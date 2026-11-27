# planetiler

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/onthegomap/planetiler, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/planetiler

## Pinned environment

- Project commit: `c078dad812089d266f24a73b8f4aaa052a6ed8c5`
- Test commit: `c078dad812089d266f24a73b8f4aaa052a6ed8c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.6 to 17.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 17.6 | 3 | 3 | [run](https://argusic.com/run/b116ab0c-8b50-4681-8b16-2cdebb0aa148) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Java 21 not found in container (no root to apt-install)`
- 1 min: `git submodule planetiler-openmaptiles not initialized (directory was empty)`
- `Maven failed to resolve ${revision} parent POM when building individual submodules without dependency chain`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
