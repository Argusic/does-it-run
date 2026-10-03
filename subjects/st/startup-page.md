# startup-page

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/timh-dev/startup-page, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/startup-page

## Pinned environment

- Project commit: `df45b47860d5c69a49bf2a1d65e119ff747e4275`
- Test commit: `df45b47860d5c69a49bf2a1d65e119ff747e4275`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.9 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 3 | 4.9 | 0 | 0 | [run](https://argusic.com/run/ddce84d9-2fac-4e96-b3cf-426f1b8abfd1) |
| 2 | pass | 100 | 3.1 | 8.1 | 2 | 2 | [run](https://argusic.com/run/b046fbbb-828f-4259-9765-623065857eea) |

## What was observed on a clean machine

Attempt 2:

- 1.8 min: `Node.js v18 insufficient (needs >=22) , installed v22.14.0 manually`
- `npm prefix cannot be changed from project config warning`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
