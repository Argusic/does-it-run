# dsh-univer-office

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dream-num/dsh-univer-office, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dsh-univer-office

## Pinned environment

- Project commit: `5ce30f6eb88cf48e24e731782020c1d811144990`
- Test commit: `5ce30f6eb88cf48e24e731782020c1d811144990`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 22.3 to 22.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 23 | 22.3 | 5 | 5 | [run](https://argusic.com/run/acd322c6-8128-4a8b-b8e8-3476e0249011) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node.js is v18.19.1 but the project requires >=22.19.0 (error TS error / pnpm 11.23.0 itself refuses v18)`
- 2 min: `pnpm is not installed inside the container`
- 5 min: `No Chrome/Chromium system browser found, so screenshot/PDF/layout tests failed to launch Chromium`
- 2 min: `repo-wide format:check fails on checked-in files src/client/conversation/univer-turn-definition.ts and test/fixtures/header.html`
- 8 min: `test/host-settings-profile.mjs requires an independently installed DSH runtime (UNIVER_DSH_RUNTIME_ROOT) which was not present`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
