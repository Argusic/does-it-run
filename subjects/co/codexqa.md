# codexqa

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openqa-cn/codexqa, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/codexqa

## Pinned environment

- Project commit: `783954281fc4898a9fac66a575363f419d4683e4`
- Test commit: `783954281fc4898a9fac66a575363f419d4683e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.7 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 5.7 | 4 | 4 | [run](https://argusic.com/run/7787f122-b462-43c7-895f-59eacda2d7ff) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `codexqa-defect-analyzer npm test failed: AssertionError 'scope_policy must list data/adhoc excludes' because PyYAML was missing, so scope_policy.yaml loaded as {}`
- 5 min: `npx skills add . --list failed on container Node 18.19.1 (styleText import from node:util, skills@1.7.4 requires node >=22.20.0; docs say Node 18+, so container is below tooling bar)`
- 3 min: `jev-browser npm test: 16/92 live Chromium tests failed 'Chromium distribution chrome is not found' (Playwright browser absent, no root for system chrome)`
- 4 min: `defect-analyzer full scan first failed EACCES on global npm install of closed-source @openqa-cn/codexqa into /usr/local (no root; auto-installer uses npm prefix -g)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
