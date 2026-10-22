# routeros-api-php

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/EvilFreelancer/routeros-api-php, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/routeros-api-php

## Pinned environment

- Project commit: `5351c0c622e06c73e1c64caca453240328b486d4`
- Test commit: `5351c0c622e06c73e1c64caca453240328b486d4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 11.7 | 5 | 5 | [run](https://argusic.com/run/5a8f2d9e-3f37-46bb-a069-a7efdb74eeff) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `No PHP runtime in container (no root to apt-install)`
- 6 min: `RouterOS device required by tests (ROS_HOST via phpunit.xml pointed at a private address)`
- 2 min: `Mock bad-credentials reply lacked terminating !done block, so client got StreamException instead of BadCredentialsException`
- 2 min: `tests/ConfigTest.php asserted 12 config parameters but Config has 13 (throw_timeout_exception added)`
- 1 min: `Mock TCP server process vanished between shell invocations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
