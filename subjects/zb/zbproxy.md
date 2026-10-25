# ZBProxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/layou233/ZBProxy, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/zbproxy

## Pinned environment

- Project commit: `5570a6aec577aefebe7704e1919732428111e5e7`
- Test commit: `5570a6aec577aefebe7704e1919732428111e5e7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.1 | 2 | 2 | [run](https://argusic.com/run/78e2d176-fd51-4c82-bcad-5e71f76826e6) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not installed in container (no root for apt)`
- `Test TestSystemOutbound_DialContextWithSRV fails: external SRV record dummy.launium.com does not resolve in this environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
