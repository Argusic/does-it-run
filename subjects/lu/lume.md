# lume

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lumeland/lume, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/lume

## Pinned environment

- Project commit: `45e80811f6ab24d050a108358234dd6d205f1d42`
- Test commit: `45e80811f6ab24d050a108358234dd6d205f1d42`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.5 to 3.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 3.5 | 1 | 1 | [run](https://argusic.com/run/99613686-1786-4569-8ad8-a7495231451d) |
| 2 | pass | 100 | 1.5 | 2.5 | 2 | 2 | [run](https://argusic.com/run/64d52a76-8975-4817-b48d-d38b9ea8ba3a) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Deno runtime not installed`

Attempt 2:

- 1 min: `deno not installed in container`
- `google_fonts.test.ts: snapshot mismatch - Google Fonts API returned different font data than expected snapshots`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
