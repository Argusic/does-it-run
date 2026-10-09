# linkinator

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JustinBeckwith/linkinator, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/linkinator

## Pinned environment

- Project commit: `1f183feb51807b91bf873a20ca946dabcd2866bd`
- Test commit: `1f183feb51807b91bf873a20ca946dabcd2866bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 2.2 | 1 | 1 | [run](https://argusic.com/run/79304e1f-4f1e-47a8-ba3e-6b71f7abfb3a) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 does not support 'with { type: 'json' }' syntax (requires Node >=22). 'node build/src/cli.js --version' failed with SyntaxError.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
