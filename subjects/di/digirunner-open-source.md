# digiRunner-Open-Source

**Verdict: could not verify.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TPIsoftwareOSPO/digiRunner-Open-Source, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/digirunner-open-source

## Pinned environment

- Project commit: `41a280195e7f448282ab2b7eb94313955425b8a4`
- Test commit: `41a280195e7f448282ab2b7eb94313955425b8a4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 8.1 to 10.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 8.1 | 1 | 1 | [run](https://argusic.com/run/73ed4dc9-baae-417d-b6b9-db1aef9587d5) |
| 2 | fail | 70 | 2 | 10.3 | 2 | 1 | [run](https://argusic.com/run/8db5f379-c19f-45b4-827a-47e88bd255ac) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Java not found in container`

Attempt 2:

- 2 min: `No JDK in container - had to download Temurin JDK 25 manually`
- `CustomJasyptEncryptor unable to load private key (config-related warning)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
