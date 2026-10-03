# animal-island-ui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/guokaigdg/animal-island-ui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/animal-island-ui

## Pinned environment

- Project commit: `29051196bd7586d4484b55431b03178e6046fa64`
- Test commit: `29051196bd7586d4484b55431b03178e6046fa64`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.3 to 19.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 19.3 | 2 | 2 | [run](https://argusic.com/run/7ba07b93-9125-40b2-9dfc-bd7259a55abf) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `jsdom@29.1.1, vitest@4, and vite@7 require Node >=20.19.0 but container provides Node 18.19.1 , fork-pool workers fail with ERR_REQUIRE_ESM and threads-pool segfaults`
- 2 min: `Vite 7 build segfaults on Node 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
