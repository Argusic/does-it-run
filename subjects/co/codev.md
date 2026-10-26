# codev

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cluesmith/codev, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codev

## Pinned environment

- Project commit: `1caf6ce92f3b1f493eb1cbe8cad5b7e0d8661dc0`
- Test commit: `1caf6ce92f3b1f493eb1cbe8cad5b7e0d8661dc0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.1 to 13.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 13.1 | 3 | 3 | [run](https://argusic.com/run/14a98d48-b062-4317-9ff3-030053c913c3) |

## What was observed on a clean machine

Attempt 1:

- `pnpm not on PATH and required for install`
- 1 min: `Node.js v18 but project requires >=20; rolldown uses node:util.styleText unavailable in 18`
- 2 min: `3 test files timing out in constrained container (session-manager, spec-755-migration, tower-cloud-cli)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
