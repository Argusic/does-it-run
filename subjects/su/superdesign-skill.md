# superdesign-skill

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/superdesigndev/superdesign-skill, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/superdesign-skill

## Pinned environment

- Project commit: `f9f05cd988c247dce6c072eaf9ac6b162f2ffc4b`
- Test commit: `f9f05cd988c247dce6c072eaf9ac6b162f2ffc4b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.8 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 5.8 | 4 | 4 | [run](https://argusic.com/run/b3fc745b-4580-4210-8d11-a23521765aa5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install -g @superdesign/cli@latest failed with EACCES (permissions on /usr/local/lib/node_modules)`
- `npm install warning: posthog-node@5.74.0 requires Node.js ^20.20.0 or >=22.22.0, current Node.js is v18.19.1`
- `npx skills add superdesigndev/superdesign-skill failed - skills CLI requires Node.js >=22.20.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
