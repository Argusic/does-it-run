# changed-files

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tj-actions/changed-files, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/changed-files

## Pinned environment

- Project commit: `9c9e94395b39f2628ceed2caba849f630866e9e0`
- Test commit: `9c9e94395b39f2628ceed2caba849f630866e9e0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.9 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 9.9 | 2 | 2 | [run](https://argusic.com/run/98150fc2-ee00-4822-88d9-1b20a02d3dd0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install peer dependency conflict (eslint-plugin-jest vs @typescript-eslint/eslint-plugin)`
- 4 min: `getPreviousGitTag tests failed because repository has no git tags with expected SHAs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
