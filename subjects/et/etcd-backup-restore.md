# etcd-backup-restore

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gardener/etcd-backup-restore, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/etcd-backup-restore

## Pinned environment

- Project commit: `e51fbc84b564702af7a71f24ef2d0d087472e6c4`
- Test commit: `e51fbc84b564702af7a71f24ef2d0d087472e6c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 41.5 to 41.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 41 | 41.5 | 2 | 2 | [run](https://argusic.com/run/e4e4b57d-9fcf-4e68-a8b9-dce6cd001bb9) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Go compiler not found in container (no root, no pre-installed go)`
- 2 min: `pkg/member/member_control_suite_test.go resolved ../../../test/output outside repo (/work/test/) which does not exist; permission denied on mkdir`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
