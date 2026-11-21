# ai-git-bot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tmseidel/ai-git-bot, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/ai-git-bot

## Pinned environment

- Project commit: `d1e8b3b5b52c71ada9ba1bc9b6f14b62bca781c8`
- Test commit: `d1e8b3b5b52c71ada9ba1bc9b6f14b62bca781c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.9 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 8.9 | 2 | 2 | [run](https://argusic.com/run/552cca58-468e-43af-8672-3d62fab1a295) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing Java 21 JDK and Maven in container`
- 2 min: `Missing OpenSSH client tools (ssh-keygen, ssh-keyscan)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
