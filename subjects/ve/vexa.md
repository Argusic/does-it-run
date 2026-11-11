# vexa

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Vexa-ai/vexa, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/vexa

## Pinned environment

- Project commit: `dba990b413bd0f888b02d46a24f802db492addbb`
- Test commit: `dba990b413bd0f888b02d46a24f802db492addbb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 17.1 to 33.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 17.1 | 6 | 6 | [run](https://argusic.com/run/3a5b4b7c-0cf2-47e3-998b-746ad5b2dc14) |
| 2 | pass with mocks | 92 | 26 | 33.6 | 3 | 3 | [run](https://argusic.com/run/89167421-b9d6-4d92-9dd7-490272d1f8ab) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 incompatible (needs >=22.13)`
- 1 min: `pnpm not found and npm install -g lacked permission`
- 1 min: `pnpm corepack signature verification failed with Node 22`
- 1 min: `Python setuptools build-backend mismatch in clients/slim/pyproject.toml`
- 1 min: `Python flat-layout package discovery error in clients/slim`
- 0.5 min: `pydantic-settings missing for core/agent tests`

Attempt 2:

- 4 min: `Node.js v18 (system) incompatible with project requirement >=22.13 , caused 'webidl-conversions' crash in @vexa/join (ArrayBuffer.prototype.resizable missing) and 'sharp' import-with crash in bot/desktop/mixed-pipeline`
- 1 min: `pnpm not installed on system`
- `@vexa/mixed-pipeline virtual-time-equivalence test has 2 pre-existing failures , virtual time heartbeat produces slightly different draft/confirm output than real time (335B vs 489B durable rows, 7 vs 6 publish calls)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
