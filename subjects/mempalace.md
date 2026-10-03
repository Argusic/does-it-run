# mempalace

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MemPalace/mempalace, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mempalace

## Pinned environment

- Project commit: `a9f345cc63254eb4dea7abad36963b85c9f8453a`
- Test commit: `a9f345cc63254eb4dea7abad36963b85c9f8453a`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 3.7 to 21.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 1 | 21.5 | 1 | 1 | [run](https://argusic.com/run/70c3b433-cde3-4feb-8846-1e761aef692b) |
| 2 | pass | 100 | 1.5 | 3.7 | 0 | 0 | [run](https://argusic.com/run/947fc7d2-4b0e-408d-8b99-c4acfd1780e0) |
| 3 | pass | 100 | 5 | 5.3 | 0 | 0 | [run](https://argusic.com/run/058bd136-7f2a-4349-9183-38c0a044ee51) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `Flaky test isolation: test_checkpoint_added_by_accepted_via_dispatch fails when run after test_stop_hook_* tests because a background subprocess holds the palace file lock. The test passes in isolation and when run within its own test class`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
