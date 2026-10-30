# tecli

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/awslabs/tecli, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/tecli

## Pinned environment

- Project commit: `eafed26c0beabf326440dce40867b9ee40cb84d5`
- Test commit: `eafed26c0beabf326440dce40867b9ee40cb84d5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 8 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 8 | 0 | 0 | [run](https://argusic.com/run/c7b21a39-efe6-44d8-9bf6-5420fb8c8c81) |
| 2 | pass with mocks | 92 | 13.3 | 13.6 | 8 | 8 | [run](https://argusic.com/run/72da3062-5753-424d-bdc7-f6229bee85d6) |

## What was observed on a clean machine

Attempt 2:

- 2.5 min: `Go 1.27.3 not installed in container`
- 0.5 min: `Missing box/blob.go (go generate needed)`
- 1 min: `os.Chdir() in test helpers leaked CWD into temp dirs, crashing subsequent os.Getwd() calls`
- 1 min: `configure controller used fmt.Println instead of cmd.Println, bypassing test output buffer in all configure tests`
- 3 min: `apply/plan/run tests passed --organization flag that doesn't exist on those subcommands, and used invalid arguments like 'list'/'create'/'delete' for apply/plan`
- 1 min: `workspace integration test passed --organization flag that doesn't exist on workspace subcommand`
- 2 min: `SSH key tests passed --organization flag that doesn't exist on ssh-key subcommand`
- 1.5 min: `TFC_TEAM_TOKEN env var required to initialize go-tfe client, causing TestGetFFEClient and API-calling tests to fatally exit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
