# open-artifact

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JimLiu/open-artifact, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-artifact

## Pinned environment

- Project commit: `425b43d42309df162d763ff40d47f513643af6fb`
- Test commit: `425b43d42309df162d763ff40d47f513643af6fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 28.9 to 31.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 28.9 | 2 | 2 | [run](https://argusic.com/run/66d7b5a9-3c11-4e22-9178-c0b655736f9b) |
| 2 | pass | 100 | 3 | 31.1 | 2 | 2 | [run](https://argusic.com/run/b1bd663f-73ee-419c-bb1c-01d347163f9e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 available but project requires >=22.18`
- 2 min: `Flaky test failures: 3 failing, 16 cancelled (all pre-existing race conditions when tests run in parallel)`

Attempt 2:

- 2 min: `Node.js 18.19.1 (below minimum 22.18) needed manual upgrade`
- `1 test failure + 16 cancelled in ownership.test.ts: cancelledByParent race in node --test with t.mock async describe`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
