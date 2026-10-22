# wag

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NHAS/wag, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/wag

## Pinned environment

- Project commit: `ff05f657364b9bbf4c4abc5643f38efee785e48f`
- Test commit: `ff05f657364b9bbf4c4abc5643f38efee785e48f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.1 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 11.1 | 4 | 4 | [run](https://argusic.com/run/e90fe1a4-c9b2-4b71-b076-d8a3de2f6179) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not found in PATH`
- 2 min: `security/pam_appl.h: No such file or directory`
- 2 min: `link: cannot find -lpam and undefined reference to audit_open`
- 3 min: `embed pattern dist/assets/*: no matching files found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
