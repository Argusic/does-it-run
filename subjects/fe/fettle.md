# fettle

**Verdict: runs.** Argusic Score 91 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mehatab/fettle, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/fettle

## Pinned environment

- Project commit: `0622c94851f75549d2286d5910057d59ec42ed8a`
- Test commit: `0622c94851f75549d2286d5910057d59ec42ed8a`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 6.8 to 11.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 6.8 | 1 | 1 | [run](https://argusic.com/run/cdd22712-a61d-4377-beac-534e68bee4cd) |
| 2 | pass | 90 | 10 | 11.6 | 2 | 1 | [run](https://argusic.com/run/5630a7ec-78f8-4443-adf7-7becea13a0f8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Invalid next.config.js: empty assetPrefix for non-production env`

Attempt 2:

- 5 min: `next export failed: 'Image Optimization using Next.js' default loader is not compatible with next export' (blocks the GitHub Pages deployment path used by .github/workflows/pages.yml)`
- 1 min: `scripts/health-check.sh ended with 'fatal: You are not currently on a branch' during git push`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
