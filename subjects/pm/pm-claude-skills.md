# pm-claude-skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mohitagw15856/pm-claude-skills, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/pm-claude-skills

## Pinned environment

- Project commit: `0246bd45ee7bd6cef57ec6fcec9dd0062c301652`
- Test commit: `0246bd45ee7bd6cef57ec6fcec9dd0062c301652`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.1 | 3.4 | 3 | 3 | [run](https://argusic.com/run/3d1e9205-97f5-4b0e-85b0-e02cd0dd8457) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `web/skills.json not found after fresh checkout , generated file missing`
- 5 min: `exports/ dirs not found , generated files missing after fresh checkout`
- 1 min: `Playwright not installed for browser tests (web-smoke.mjs, xss-fuzz.mjs)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
