# freehire

**Verdict: runs.** Argusic Score 94 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/strelov1/freehire, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/freehire

## Pinned environment

- Project commit: `900408d7e3172193966064f096b4dbf4e5d78b2a`
- Test commit: `900408d7e3172193966064f096b4dbf4e5d78b2a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 28.7 to 46.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 44 | 46.1 | 5 | 4 | [run](https://argusic.com/run/826e9b2f-a20d-4b28-b586-b1248bf1f311) |
| 2 | pass with mocks | 92 | 22 | 28.7 | 2 | 2 | [run](https://argusic.com/run/f2c90700-a2de-4f2a-903d-a8b39b5966cb) |

## What was observed on a clean machine

Attempt 1:

- 30 min: `go, pnpm, postgres, redis, meilisearch, poppler not on base image`
- 5 min: `web vitest fails with 'Tsconfig not found' / could not resolve node:module`
- 6 min: `go test ./internal/api/handler fails on PDF resume tests (status 400) when pdftotext not on PATH`
- 3 min: `cmd/billing-sync TestTheStoreProviderAloneKeepsTheWorkerRunning fails (run stops at gate with RevenueCat configured)`
- `background children died with exec session; later server instances killed by harness`

Attempt 2:

- 2 min: `Go compiler not found in environment`
- 5 min: `pdftotext binary not found (poppler-utils) , two handler tests failed (TestRoastCV_RealPDFFromAnAnonymousCaller, TestExtractResumeProfile_PDF)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
