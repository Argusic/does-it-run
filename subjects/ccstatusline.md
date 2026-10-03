# ccstatusline

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sirmalloc/ccstatusline, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ccstatusline

## Pinned environment

- Project commit: `68eb01e40d0e480a7e0297a638639185637208a3`
- Test commit: `68eb01e40d0e480a7e0297a638639185637208a3`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 5.1 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.5 | 5.1 | 2 | 2 | [run](https://argusic.com/run/3da3ae8a-cc96-4710-bc3f-50d697536d01) |
| 2 | pass | 100 | 2 | 5.4 | 0 | 0 | [run](https://argusic.com/run/1696f772-1827-4f34-b2d4-1cf658ff5b78) |
| 3 | pass | 100 | 6 | 6 | 4 | 4 | [run](https://argusic.com/run/5d3f611a-edc7-4460-a049-f5edabfda997) |

## What was observed on a clean machine

Attempt 1:

- 3.5 min: `Bun not pre-installed in container`
- 1 min: `unzip not installed (needed by official bun installer)`

Attempt 3:

- 2 min: `bun: not found`
- 1 min: `npm ERESOLVE peer dependency conflict with eslint-plugin-react`
- 1 min: `TypeScript errors in git-review-cache.test.ts readFileSync overload assignment`
- `ESLint 10.x crashes on Node 18 (util.styleText not a function)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
