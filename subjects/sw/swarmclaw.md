# swarmclaw

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/swarmclawai/swarmclaw, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/swarmclaw

## Pinned environment

- Project commit: `ed38ba5329c20e48c03b4a4028f4a76a1a75e2d1`
- Test commit: `ed38ba5329c20e48c03b4a4028f4a76a1a75e2d1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 43 | 9.1 | 3 | 3 | [run](https://argusic.com/run/446981ee-11a2-41e2-bb6a-eacb837c4798) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `System Node was v18.19.1 but the project requires Node >=22.6, and setup.hard-fails on older Node`
- 8 min: `127.0.0.1 loopback refused connections inside the container (container-level network namespace allows only the container IP)`
- 5 min: `Electron main process launches but tried to load http://127.0.0.1:3456 and initially hit ERR_CONNECTION_REFUSED`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
