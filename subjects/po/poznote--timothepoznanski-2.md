# Poznote

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/timothepoznanski/Poznote, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/e7be3a3e-17d3-4c57-80fb-c72027e57127

## Pinned environment

- Project commit: `58fd177585f0d1cf064190e11c214c89f4f01a09`
- Test commit: `58fd177585f0d1cf064190e11c214c89f4f01a09`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.8 to 16.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 12.8 | 3 | 3 | [run](https://argusic.com/run/e7be3a3e-17d3-4c57-80fb-c72027e57127) |
| 2 | pass | 100 | 18 | 16.7 | 1 | 1 | [run](https://argusic.com/run/3c9e4110-bc7b-437a-bd92-08aeafa18245) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP interpreter installed in container`
- 2 min: `MCP server missing service token at standard path`
- 1 min: `Node.js v18.19.1 too old for Vite 8 build (needs node:util.styleText from Node 20+)`

Attempt 2:

- 8 min: `PHP 8.3 CLI SAPI incompatible with PHP 8.5 FPM SAPI: namespace class Pdo\Sqlite not found and PDO::createFunction() not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
