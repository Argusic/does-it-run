# soundcli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/baairon/soundcli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/soundcli

## Pinned environment

- Project commit: `4f63c35d6511476f9dc11553d99f524d20252ab7`
- Test commit: `4f63c35d6511476f9dc11553d99f524d20252ab7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.1 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 2.1 | 1 | 1 | [run](https://argusic.com/run/bdbd0fd8-7d4b-41cc-a913-3945b18a38c7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing optional native binding @rolldown/binding-linux-x64-gnu required by rolldown (dependency of vitest) , npm did not install it from package-lock.json`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
