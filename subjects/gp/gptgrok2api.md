# gptGrok2api

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AuuCoder/gptGrok2api, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gptgrok2api

## Pinned environment

- Project commit: `4adce806b3a1f0ef167e21385c2b78399e07af7c`
- Test commit: `4adce806b3a1f0ef167e21385c2b78399e07af7c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12.5 | 14 | 3 | 3 | [run](https://argusic.com/run/060f342c-675c-4bbb-843c-bcd74ecde02d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python 3.13 required but not found`
- 2 min: `uv not installed in container`
- 3 min: `.env dummy auth key overrode config.json auth key at runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
