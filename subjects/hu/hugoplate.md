# hugoplate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zeon-studio/hugoplate, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/hugoplate

## Pinned environment

- Project commit: `2f5a454ee708f5f2666414af9ef48df65570752a`
- Test commit: `2f5a454ee708f5f2666414af9ef48df65570752a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 6 | 5 | 5 | [run](https://argusic.com/run/df98d822-372c-4208-88ee-b49e6d7af102) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `pnpm not pre-installed; installed via npm --prefix`
- 0.5 min: `Hugo not pre-installed`
- 3 min: `Go not pre-installed (needed for Hugo modules)`
- 0.7 min: `@tailwindcss/oxide-linux-x64-gnu native binding missing (pnpm optional deps issue)`
- 1 min: `Repo was in theme-setup mode (exampleSite/ with no themes/)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
