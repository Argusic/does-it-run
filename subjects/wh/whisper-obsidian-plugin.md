# whisper-obsidian-plugin

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nikdanilov/whisper-obsidian-plugin, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/whisper-obsidian-plugin

## Pinned environment

- Project commit: `0a0a5e409f737a9920af1430024a601d99e0b8b3`
- Test commit: `0a0a5e409f737a9920af1430024a601d99e0b8b3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.3 to 1.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.4 | 1.3 | 1 | 1 | [run](https://argusic.com/run/9436c131-ec6f-4de6-9373-dbee8ac4ffb7) |

## What was observed on a clean machine

Attempt 1:

- 0.4 min: `npm install failed due to peer dependency conflict with @types/node v16 and vitest 2.x on Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
