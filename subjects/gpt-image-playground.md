# gpt_image_playground

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CookSleep/gpt_image_playground, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/gpt-image-playground

## Pinned environment

- Project commit: `326fdd112e599c280bb3fa29a9e707fecd9dbca7`
- Test commit: `326fdd112e599c280bb3fa29a9e707fecd9dbca7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17 to 17 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 17 | 1 | 1 | [run](https://argusic.com/run/b4829a0b-07c3-4013-91ec-ee45ead44eea) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `npm install failed due to Node.js version incompatibility (v18.19.1 vs required >=20) , wrangler's esbuild postinstall script errored and vitest 4.x/jsdom 29.x require Node >=20`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
