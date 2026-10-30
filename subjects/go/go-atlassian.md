# go-atlassian

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ctreminiom/go-atlassian, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/go-atlassian

## Pinned environment

- Project commit: `78492cd9e3626c6901cfb4be7a364d17ae851168`
- Test commit: `78492cd9e3626c6901cfb4be7a364d17ae851168`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 4.1 | 2 | 2 | [run](https://argusic.com/run/64caf63e-9fe6-4bd9-b453-b544f6705ac8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go toolchain missing on PATH (go: not found)`
- `Initial e2e probe used wrong Assets/Confluence API signatures; Assets client returned 404 for a misrouted mock path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
