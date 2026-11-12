# primo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/primocms/primo, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/primo

## Pinned environment

- Project commit: `f6fe55b1699992143bddf526c04f1eb8ac68dcca`
- Test commit: `f6fe55b1699992143bddf526c04f1eb8ac68dcca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10.9 to 44.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 10.9 | 4 | 4 | [run](https://argusic.com/run/ecb35595-7f02-4487-b4ce-5fd28987720e) |
| 2 | pass | 100 | 43 | 44.2 | 4 | 4 | [run](https://argusic.com/run/7c13e3aa-123e-45ea-95f4-e0f4aaf8d24b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 is below the required ^22.17.0`
- 1 min: `Go not found in PATH`
- 1 min: `go build failed: pattern build/*: no matching files found`
- 1 min: `go build failed: pattern common/index.cjs: no matching files found`

Attempt 2:

- 2 min: `Node.js 18 installed, requires ^22.17.0`
- 1 min: `Go compiler not installed, required version 1.26.10`
- 1 min: `Frontend vite build OOM-killed with 1.9GB RAM when run concurrently with other builds`
- `Go test suite (go test ./...) runs for >10 minutes sequentially and exceeds reasonable time budget on this hardware`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
