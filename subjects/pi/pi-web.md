# pi-web

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jmfederico/pi-web, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-web

## Pinned environment

- Project commit: `92d3eee60a508abc2f53f9e6a79dcaef2273e3d9`
- Test commit: `92d3eee60a508abc2f53f9e6a79dcaef2273e3d9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28 to 28 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 28 | 4 | 4 | [run](https://argusic.com/run/8854b11b-525f-4244-8555-34cc22287887) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node 18 present but project requires >=22.19; installed user-space Node 22.19.0 for all verification.`
- 7 min: `pi-web install/doctor fail: no systemd user bus in this container (systemd refuses to run a user instance without systemd PID 1); native systemd user services cannot be managed here.`
- 1 min: `Initial mock returned a non-stream JSON body for requested SSE stream, so the agent loop retried; not a product bug.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
