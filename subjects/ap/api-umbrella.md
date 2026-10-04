# api-umbrella

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NatLabRockies/api-umbrella, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/api-umbrella

## Pinned environment

- Project commit: `b3fbd68d6fa2bf5d811fde9b2c369b3558a77069`
- Test commit: `b3fbd68d6fa2bf5d811fde9b2c369b3558a77069`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 12.5 to 27 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 12.5 | 0 | 0 | [run](https://argusic.com/run/e98d61f4-e335-414e-8116-f23debf37985) |
| 2 | fail | 20 | 45 | 27 | 5 | 5 | [run](https://argusic.com/run/844d7f49-cf77-4e96-a5ec-1970cf4ceb68) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `Build failed at deps:fluent-bit: Fluent Bit compilation from source needs flex/bison/libyaml-dev, not installed and cannot be installed without root`
- 1 min: `rsync not found`
- 2 min: `npm install -g fails without root`
- 1 min: `PNPM_HOME unbound variable`
- 1 min: `chrpath not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
