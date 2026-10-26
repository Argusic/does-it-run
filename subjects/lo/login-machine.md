# login-machine

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RichardHruby/login-machine, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/login-machine

## Pinned environment

- Project commit: `e1da92965029ce23bfc372f4483ed7c55ba84736`
- Test commit: `e1da92965029ce23bfc372f4483ed7c55ba84736`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.8 to 16.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 17 | 16.8 | 4 | 4 | [run](https://argusic.com/run/511e82de-0d55-47b8-9199-d5c298d502f8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Next.js 16 requires Node.js >=20.9.0, but only Node.js v18.19.1 was available`
- 4 min: `BROWSERBASE_API_KEY and BROWSERBASE_PROJECT_ID env vars not set , browser.ts threw errors on startup`
- 1 min: `Two ESLint warnings: unused variables 'url' and 'hasInput' in the new mock code`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
