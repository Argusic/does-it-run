# gh-skyline

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/github/gh-skyline, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gh-skyline

## Pinned environment

- Project commit: `5245b2fc95250075cac37d24a4cd9b09258de5a8`
- Test commit: `5245b2fc95250075cac37d24a4cd9b09258de5a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18.7 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 18.7 | 4 | 4 | [run](https://argusic.com/run/3eb93747-8643-4320-82c3-41e66a7c4996) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `Go toolchain missing in container (no root to apt-install)`
- 3 min: `GitHub CLI missing (needed per README)`
- 3 min: `App requires GitHub GraphQL auth; GH_TOKEN alone still hit api.github.com so mock could not be reached`
- 1 min: `gh extension install . fails because clone dir is named 'repo' not 'gh-skyline'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
