# DS-Bot

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Fei-Craft/DS-Bot, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/run/b073e6de-463e-47d7-9833-7bd7b5746c9d

## Pinned environment

- Project commit: `d104d9ca18d69a35460f14e15dff4d553181433a`
- Test commit: `d104d9ca18d69a35460f14e15dff4d553181433a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 8 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 8.4 | 3 | 3 | [run](https://argusic.com/run/b073e6de-463e-47d7-9833-7bd7b5746c9d) |
| 2 | pass with mocks | 92 | 64 | 8 | 4 | 4 | [run](https://argusic.com/run/d5591f02-7850-47e6-a6fe-cfca5b29b433) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 pre-installed but project requires >=22.19.0`
- `App test: 1 failure , ws@8.23.0 is a peer dep of @earendil-works/pi-ai but app/package.json declares ws@8.18.3`
- `Desktop app: runtime Node not found at build/runtime/primary-runtime/dependencies/node/bin/node`

Attempt 2:

- 5 min: `Node.js v18 too old for DSH (needs >=24.9.0)`
- 1 min: `pnpm not found for bench.sh`
- `esbuild postinstall not covered by allowScripts`
- 1 min: `DSH harness packages had unapproved install scripts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
