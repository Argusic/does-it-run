# patchright-nodejs

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Kaliiiiiiiiii-Vinyzu/patchright-nodejs, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/patchright-nodejs

## Pinned environment

- Project commit: `9d5f0ecf20f305784a2c5a1a3226299e82daba83`
- Test commit: `9d5f0ecf20f305784a2c5a1a3226299e82daba83`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 15 | 2.9 | 2 | 1 | [run](https://argusic.com/run/fe94da2f-6f79-4963-9319-0dab0319f6e9) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `npx patchright install chromium and patched-browser launch fail under container system Node 18.19.1: "Playwright requires Node.js 20 or higher"; patchright@1.63.0 declares engines node>=20`
- 1 min: `patchright_rebranding.ts (rebuild script) fails with FileNotFoundError: packages/playwright-core/types/types.d.ts because the repo ships this patch-source without the required full Playwright checkout (packages/playwright-core is created on`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
