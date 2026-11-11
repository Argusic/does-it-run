# genie

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/automagik-si/genie, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/genie

## Pinned environment

- Project commit: `1d6eb08ba67a9df43600d05fa45779e90bd82ccc`
- Test commit: `1d6eb08ba67a9df43600d05fa45779e90bd82ccc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 64.1 to 64.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 49 | 64.1 | 4 | 4 | [run](https://argusic.com/run/46ae8659-f692-4630-ab12-d8cf21762f8d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `bunx not in PATH (bun install puts bun binary but not bunx symlink)`
- 4 min: `NO_COLOR=1 in host env causes FORCE_COLOR tests to always fail because NO_COLOR wins over FORCE_COLOR in colorEnabled()`
- `plugin build tests fail because Node 18 cannot run .ts files directly; node build.ts fails with ERR_UNKNOWN_FILE_EXTENSION`
- `23 installer/infrastructure tests fail because they require real genie binary installed in the environment, which isn't present in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
