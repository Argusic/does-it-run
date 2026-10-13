# metatube-sdk-go

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/metatube-community/metatube-sdk-go, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/metatube-sdk-go

## Pinned environment

- Project commit: `19a92ad3263ab7b69636d26d7cc32f531c0a0804`
- Test commit: `19a92ad3263ab7b69636d26d7cc32f531c0a0804`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 8.6 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3 | 17.7 | 4 | 4 | [run](https://argusic.com/run/ecf47b25-3d03-4adc-aa12-88508541ecee) |
| 2 | fail | 20 | n/a | 8.6 | 0 | 0 | [run](https://argusic.com/run/2f5d8b43-fd38-4ca0-b26b-0e84c5039c14) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.26 not installed in container`
- `Provider tests fail due to external sites being unreachable (aventertainments, duga, faleno, fanza, fc2, fc2hub, fc2ppvdb, gcolle, getchu, gfriends, jav321, javbus, javfree, kin8tengoku, mgstage, pcolle, sod, tokyo-hot)`
- `engine/dbengine test fails: Docker socket not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
