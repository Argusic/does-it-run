# openmeld

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amplifthq/openmeld, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openmeld

## Pinned environment

- Project commit: `82643a14b038c0cff4937a488833c3a43214e248`
- Test commit: `82643a14b038c0cff4937a488833c3a43214e248`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 49.5 to 49.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 49.5 | 5 | 5 | [run](https://argusic.com/run/49304d25-8694-4a24-9df3-91c8502980be) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18 in the environment but repo requires Node 24`
- `pnpm/corepack not available with system Node`
- 15 min: `pnpm build hangs, local-resources memory admission denies heavy build in container with 8GiB constrained memory and 1.6GiB available`
- 1 min: `openmeld-web build fails: cannot resolve origin/main (shallow clone)`
- `25 of 3535 CLI test failures and 4 of 1765 schemas test failures are pre-existing repo-internal test/source drift`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
