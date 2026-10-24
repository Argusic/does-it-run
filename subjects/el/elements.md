# elements

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/muxinc/elements, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/elements

## Pinned environment

- Project commit: `276bc445450d69885e64b291312d78204a8f87b5`
- Test commit: `276bc445450d69885e64b291312d78204a8f87b5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.7 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 17.7 | 3 | 3 | [run](https://argusic.com/run/b3ce05a0-5b88-4e4a-b887-92df5fa18918) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm9 cannot parse lockfile: dependency downlevel-dts declares typescript@"next" (invalid semver)`
- 1 min: `All web-test-runner configs used playwrightLauncher with channel:'chrome' but no system Chrome installed`
- 1 min: `mux-active-viewer-count uses puppeteer-core chromeLauncher which needs --no-sandbox in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
