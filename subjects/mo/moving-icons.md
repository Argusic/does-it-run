# Moving Icons

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jis3r/icons, licensed MIT, written in Svelte.

Evidence and recordings: https://argusic.com/subject/moving-icons

## Pinned environment

- Project commit: `eebffac1dc7944f844c459ec634bf8d9af38d11f`
- Test commit: `eebffac1dc7944f844c459ec634bf8d9af38d11f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 4.7 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 7.3 | 2 | 2 | [run](https://argusic.com/run/0643ccad-d7cd-432e-a19a-724d26fe45d9) |
| 1 | pass | 100 | 7.2 | 8.2 | 5 | 5 | [run](https://argusic.com/run/f44648af-bbb5-4918-adbf-37e35e01be5f) |
| 2 | pass | 100 | 12 | 6.3 | 2 | 2 | [run](https://argusic.com/run/60f87d1b-69f7-41f6-ba65-76f9af4c593f) |
| 3 | pass | 100 | 0.2 | 4.7 | 1 | 1 | [run](https://argusic.com/run/c6a6a842-d51a-4335-9907-9691684c7273) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `.npmrc had engine-strict=true which blocked npm install on Node 18 (container default)`
- 4 min: `Node 18 is too old for vite 8/vitest 4 (require Node 20+)`

Attempt 1:

- 0.5 min: `Node 18 engine-strict blocks install, needs Node >=20.19`
- 0.3 min: `Missing @tailwindcss/oxide-linux-x64-gnu native binding (npm optional deps bug)`
- 0.3 min: `Vite 8 / Vitest 4 require Node 20 (styleText API)`
- 0.2 min: `jsdom 29 requires node:util export styleText, CJS require of ESM module @exodus/bytes on Node 18`
- 0.5 min: `$state rune used in .ts test file, Svelte 5 requires .svelte.ts extension`

Attempt 2:

- 3 min: `engine-strict=true in .npmrc blocks npm install on Node 18 (required Node >=20 for many transitive deps)`
- 2 min: `svelte-kit sync fails on Node 18: rolldown requires node:util.styleText (Node 22+)`

Attempt 3:

- 0.5 min: `node v18.19.1 is too old - @asamuzakjp/css-color requires ^20.19.0 || ^22.12.0 || >=24.0.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
