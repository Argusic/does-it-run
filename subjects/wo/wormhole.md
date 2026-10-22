# wormhole

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MuhammadHananAsghar/wormhole, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/wormhole

## Pinned environment

- Project commit: `c53fd29e3eb46c7d41f4af21d053a3c3746fe9aa`
- Test commit: `c53fd29e3eb46c7d41f4af21d053a3c3746fe9aa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 12.3 | 3 | 3 | [run](https://argusic.com/run/fbecdc60-7877-40e2-a170-af6ef233f3ad) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain missing (go 1.26.1+ required by README, none installed)`
- 2 min: `Edge test suite crashed on Node 18 with ReferenceError: File is not defined (undici needs Node >=20)`
- 10 min: `Relay URL hardcoded as wss://relay.wormhole.bar with no override; /etc/hosts not writable so a local schema-correct mock relay could not be reached`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
