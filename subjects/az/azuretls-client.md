# azuretls-client

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Noooste/azuretls-client, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/azuretls-client

## Pinned environment

- Project commit: `756acc9409a45f32c97548b2fc37b77130c4f1de`
- Test commit: `756acc9409a45f32c97548b2fc37b77130c4f1de`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.2 to 6.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 6.2 | 2 | 2 | [run](https://argusic.com/run/fdaaba91-16f6-4cc0-b911-16878954d4c2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 5 min: `TestHeaderOrderHTTP3 failed: json cannot unmarshal array into Go struct field .http3.headers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
