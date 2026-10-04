# toolhive

**Verdict: runs.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/stacklok/toolhive, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/toolhive

## Pinned environment

- Project commit: `88bb28433ae7968027a624f579050b62ce380972`
- Test commit: `88bb28433ae7968027a624f579050b62ce380972`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 55 to 55 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 88 | 55 | 55 | 5 | 2 | [run](https://argusic.com/run/e338efea-f45d-41a1-a64c-cbd866c30872) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go compiler (golang) not found in container , no go binary in PATH`
- 5 min: `Task runner (go-task) not installable , dependency name mismatch in go-task's go.mod`
- `API tests fail , require Docker container runtime (pkg/api)`
- `bodylimit test hangs indefinitely (pkg/bodylimit)`
- `Keyring test fails , no system keyring provider available (pkg/secrets/keyring)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
