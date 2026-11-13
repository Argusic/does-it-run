# intent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/intent-hq/intent, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/intent

## Pinned environment

- Project commit: `39e2b86821f3ebbc5be85c52437f8440669a4fd4`
- Test commit: `39e2b86821f3ebbc5be85c52437f8440669a4fd4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 70.9 to 70.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 70.9 | 3 | 3 | [run](https://argusic.com/run/d910bf39-b314-45ce-a2cf-2e94041b02eb) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `bootstrap-dev-host failed because Node 24 and system packages (gh, shellcheck) require root for apt-get`
- 2 min: `ACP callback fixture requires Node v24.21.0 but the build used v24.22.3`
- 1 min: `make test-intentd rebuilds all crates into a separate target directory, exceeding the time budget`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
