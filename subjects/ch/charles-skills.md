# charles-skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LemonFace0309/charles-skills, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/charles-skills

## Pinned environment

- Project commit: `652fcfe0fe68888f950220a572fae3d5e9db1cdb`
- Test commit: `652fcfe0fe68888f950220a572fae3d5e9db1cdb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.4 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.1 | 2.4 | 1 | 1 | [run](https://argusic.com/run/60ada57b-b0e6-4bc6-b2f5-fe2aeeb7b2d2) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `npx skills requires Node >=22.20.0 but environment has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
