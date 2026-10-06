# openclaw-android

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aidanpark/openclaw-android, licensed MIT, written in Kotlin.

Evidence and recordings: https://argusic.com/run/89e91933-14e3-4d9a-b02f-5ff2bf7d5155

## Pinned environment

- Project commit: `cfb0740fc0961f1dd1c2a22ecf133eae443fa96f`
- Test commit: `cfb0740fc0961f1dd1c2a22ecf133eae443fa96f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.9 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 9.3 | 0 | 0 | [run](https://argusic.com/run/89e91933-14e3-4d9a-b02f-5ff2bf7d5155) |
| 2 | pass | 100 | 6 | 6.9 | 3 | 3 | [run](https://argusic.com/run/490e84ce-698a-40b5-a6cb-7a5e90bc2004) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `System Node.js v18.19.1 too old for openclaw (requires >=24.16.0)`
- 1 min: `npm install -g failed: EACCES permission denied on /usr/local/lib/node_modules`
- 2 min: `x86_64 host is not Android/Termux; installer scripts expect $PREFIX and Android environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
