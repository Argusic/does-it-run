# kitesurf

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudflare/kitesurf, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kitesurf

## Pinned environment

- Project commit: `4a2903813a22b08d4f3cc64a4b35339d0293a5d1`
- Test commit: `4a2903813a22b08d4f3cc64a4b35339d0293a5d1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 34.3 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/8118de56-34dc-4cdb-a0f2-4f87350755ce) |
| 2 | pass | 100 | 46 | 34.3 | 2 | 2 | [run](https://argusic.com/run/a5b110f6-6280-45f5-84e5-fcdd3111dfd8) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Node.js was v18.19.1 (needs 22+), pnpm and Bazelisk were not installed`
- 2 min: `Port 8787 was already occupied by an unresponsive proxy`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
