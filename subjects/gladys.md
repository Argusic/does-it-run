# Gladys

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GladysAssistant/Gladys, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/gladys

## Pinned environment

- Project commit: `8574722f2ffb1fafc10868396cfefd38a1880586`
- Test commit: `8574722f2ffb1fafc10868396cfefd38a1880586`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 82.8 to 82.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 82.8 | 7 | 7 | [run](https://argusic.com/run/e91270db-dbb6-4f45-a6a2-0adddb6b2f38) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `energy-monitoring service uuid@13 is ESM-only, breaking require()`
- 1 min: `matter service missing @matter/nodejs dep`
- 3 min: `matter service depends on @noble/curves ESM, crashes Node 18`
- 1 min: `netatmo/service uses undici v7 requires Node 20+`
- 1 min: `mcp service uses @toon-format/toon ESM-only, breaks Node 18`
- 1 min: `front build OOM`
- `sqlite3 CLI missing for gateway backup tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
