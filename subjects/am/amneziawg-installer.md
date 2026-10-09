# amneziawg-installer

**Verdict: runs.** Argusic Score 85 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bivlked/amneziawg-installer, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/amneziawg-installer

## Pinned environment

- Project commit: `d05781226c815954372899786fdc5a8b01029c7a`
- Test commit: `d05781226c815954372899786fdc5a8b01029c7a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 36.1 to 60.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 70 | 60 | 60.4 | 2 | 1 | [run](https://argusic.com/run/05db43fb-0f83-42cd-a310-d24deb1394ae) |
| 2 | pass | 100 | 8 | 36.1 | 2 | 2 | [run](https://argusic.com/run/e22b34cf-afa5-4df6-9880-7055165d9721) |

## What was observed on a clean machine

Attempt 1:

- `gpg binary not installed , 4 PPA key tests fail. Container has only gpgv (verify-only); installing gnupg requires root.`
- `git tags not fetched , 4 SHA pin lockstep tests initially failed. Fixed mid-session by running git fetch --tags.`

Attempt 2:

- 5 min: `Test test_ppa_key_embedded.bats failed because gpg-agent was not running in the test's temp GNUPGHOME`
- `qrencode binary not available - 1 test skipped`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
