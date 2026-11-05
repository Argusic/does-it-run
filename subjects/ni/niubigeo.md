# niubigeo

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Albert-Weasker/niubigeo, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/niubigeo

## Pinned environment

- Project commit: `8bc65e9d90939a8bb4a7cf694f477cac7ce89d15`
- Test commit: `8bc65e9d90939a8bb4a7cf694f477cac7ce89d15`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 7.5 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 12.6 | 3 | 3 | [run](https://argusic.com/run/162594b7-9c97-452e-b82a-4afaf1fb884f) |
| 2 | pass with mocks | 92 | 10 | 7.5 | 2 | 2 | [run](https://argusic.com/run/5ea1550f-57a7-4cc0-b572-c0a3cc1f5771) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Container has Node 18 but project requires Node >=22`
- 8 min: `Node 22.0.0 has globalThis.fetch as a getter; t.mock.method(globalThis, 'fetch') throws TypeError`
- 2 min: `Leftover node_modules_old directory was scanned by the regex constraint test, causing 1 false failure`

Attempt 2:

- 3 min: `Node.js 18 installed but project requires >=22`
- 7 min: `4 tests failed with TypeError: The argument 'methodName' must be a method`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
