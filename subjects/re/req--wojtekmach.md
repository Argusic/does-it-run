# req

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wojtekmach/req, licensed Apache-2.0, written in Elixir.

Evidence and recordings: https://argusic.com/run/03030714-6697-4bb0-91f4-83b7f76c9287

## Pinned environment

- Project commit: `58e94146b446205a4db2ebcacbe8e918fc691a6a`
- Test commit: `58e94146b446205a4db2ebcacbe8e918fc691a6a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.6 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 14.6 | 1 | 1 | [run](https://argusic.com/run/03030714-6697-4bb0-91f4-83b7f76c9287) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `:json module (OTP 27+) not available on OTP 25`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
