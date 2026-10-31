# hipocampus

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kevin-hs-sohn/hipocampus, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/hipocampus

## Pinned environment

- Project commit: `df88ca19d42a3aba4caeaba4512da46cae7827da`
- Test commit: `df88ca19d42a3aba4caeaba4512da46cae7827da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 1.9 to 1.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 1.9 | 2 | 2 | [run](https://argusic.com/run/a561ffb3-9475-4056-8fa4-b51e72df314c) |

## What was observed on a clean machine

Attempt 1:

- `npm install -g @tobilu/qmd failed , requires Node.js >=22.0.0 (container has v18.19.1) and EACCES on /usr/local/lib/node_modules`
- `npm link fails EACCES , cannot symlink into /usr/local/lib/node_modules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
