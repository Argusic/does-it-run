# pi-pocket

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TannerMidd/pi-pocket, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-pocket

## Pinned environment

- Project commit: `ed50991eb9c9b92e717f819073de36633bf83425`
- Test commit: `ed50991eb9c9b92e717f819073de36633bf83425`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.6 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 5.6 | 2 | 2 | [run](https://argusic.com/run/8b4ab1c1-363d-491e-afd5-fbc43a4ce2a9) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Ship node is v18.19.1 but Pi Pocket requires >=22.19 and bin/pi-pocket.js exits on it`
- 1 min: `Port 8787 was already occupied by the host gateway on 127.0.0.1, so the first launch attempt could not bind`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
