# procoder

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/azrtydxb/procoder, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/procoder

## Pinned environment

- Project commit: `e6997288983e5f0dd8748f1a5c7574cb11a4b961`
- Test commit: `e6997288983e5f0dd8748f1a5c7574cb11a4b961`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 20 | 7.2 | 5 | 4 | [run](https://argusic.com/run/fa92807f-194c-4538-bf28-834c7e5d61d2) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `no Go toolchain in container (go.mod pins go1.26.7); 'go' not on PATH`
- 3 min: `eslint 6.4.0 on PATH rejected --no-config-lookup used by lint code (needs eslint >=9), failing internal/lint tests`
- 3 min: `Node 18.19.1 cannot load ESM-syntax .js adapters, failing portability adapter test (needs Node >=20.19/>=22)`
- 3 min: `typescript-eslint package absent, failing TS baseline lint tests`
- 3 min: `16 pinned procoder tools (gitleaks, semgrep, golangci-lint, ruff, etc.) missing; no root to install system packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
