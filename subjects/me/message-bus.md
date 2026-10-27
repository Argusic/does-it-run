# message-bus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vardius/message-bus, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/message-bus

## Pinned environment

- Project commit: `f00c844722449aa7950c1f0f5e919a4f2db147b2`
- Test commit: `f00c844722449aa7950c1f0f5e919a4f2db147b2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 6 | 3 | 3 | [run](https://argusic.com/run/54e3907b-f528-4ef8-b223-312fc214bf4f) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Go toolchain not present (no root to apt-get install; project requires Go 1.26+)`
- 1 min: `apt-get install golang-go failed: dpkg lock permission denied (non-root container)`
- 1 min: `examples/shutdown (HTTP server) bound localhost:8080 which was in use`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
