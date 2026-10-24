# gitstream

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/linear-b/gitstream, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/gitstream

## Pinned environment

- Project commit: `5cd1030bdf52dc2580cae167e38e2d4f24da4de2`
- Test commit: `5cd1030bdf52dc2580cae167e38e2d4f24da4de2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 3.4 | 1 | 1 | [run](https://argusic.com/run/a9cc9707-7114-4c51-98d9-947d208e25b6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `plugins/filters/getCodeowners/index.js requires @octokit/rest which was not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
