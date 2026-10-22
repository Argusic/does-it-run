# ui-builder

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/olliethedev/ui-builder, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ui-builder

## Pinned environment

- Project commit: `bc1ceda306935bba87c2760fd213725f9133013b`
- Test commit: `bc1ceda306935bba87c2760fd213725f9133013b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.7 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.4 | 5.7 | 1 | 1 | [run](https://argusic.com/run/01cbe695-d678-49af-83a5-e9f8d0c6ba2f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js is v18.19.1 but Next.js 16 requires >=20.9.0. npm install warned on engine but succeeded. next dev and next build would fail under Node 18.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
