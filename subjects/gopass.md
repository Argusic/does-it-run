# gopass

**Verdict: runs.** Argusic Score 95.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gopasspw/gopass, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gopass

## Pinned environment

- Project commit: `e2dd748cdbe12829f51f3e79035a11401e939616`
- Test commit: `e2dd748cdbe12829f51f3e79035a11401e939616`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 16.9 to 25.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 17 | 16.9 | 4 | 3 | [run](https://argusic.com/run/e1512d43-787e-4b69-abb9-87ec9e675caf) |
| 2 | pass | 100 | 25 | 25.8 | 4 | 4 | [run](https://argusic.com/run/24c15fc6-55c3-47df-84cf-7d024e0538c3) |
| 3 | pass | 100 | 16 | 18.3 | 5 | 5 | [run](https://argusic.com/run/0225d5a6-4954-45d9-abf7-96003db62bd7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go (1.25.0) not installed in the container`
- 2 min: `gpg binary not found (only gpgv present)`
- 1 min: `git user identity not configured - tests fail on commit`
- `TestAgentUnlock fails - age agent socket not available`

Attempt 2:

- 1 min: `Go compiler not found in PATH`
- 3 min: `gpg, gpg-agent, gpgconf binaries not found`
- 2 min: `gpg-agent could not start: hardcoded path /usr/bin/gpg-agent`
- 1 min: `TestUpdateWorkflows failed: git user unset`

Attempt 3:

- 3 min: `Go >=1.25 not in system repos (apt has 1.22-1.24)`
- 4 min: `gpg binary not found (no root for apt install)`
- 2 min: `gpg-agent multi-call binary misidentified by argv[0], causing 'invalid option --yes' test failures`
- 2 min: `pinentry-curses needs a real TTY and fails with 'isatty' error`
- 1 min: `age setup generates a random passphrase that the pinentry wrapper doesn't know`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
