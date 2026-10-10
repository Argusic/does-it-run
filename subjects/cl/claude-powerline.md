# claude-powerline

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Owloops/claude-powerline, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claude-powerline

## Pinned environment

- Project commit: `9e9b17f9c05b91899c517b32ee7d5bf6e7f5ce36`
- Test commit: `9e9b17f9c05b91899c517b32ee7d5bf6e7f5ce36`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 7 | 6.5 | 4 | 3 | [run](https://argusic.com/run/ab1ca489-9bef-4bf4-8e6e-2a1a23cbf808) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm run build crashed on Node 18: rolldown imports node:util.styleText, which needs Node >= 20.12 (container has v18.19.1)`
- 1 min: `Build then failed with MODULE_NOT_FOUND for rolldown-binding.linux-x64-gnu.node after the original npm ci; optional dep @rolldown/binding-linux-x64-gnu was not installed under Node 18`
- 5 min: `2 of 414 tests failed (colors.test.ts NO_COLOR-empty case, core.test.ts color-code assertion) because the container harness sets NO_COLOR=1 and stdout is a non-TTY, so getColorSupport() resolves to 'none'; the repo's own CI (.github/workflo`
- 1 min: `npm run benchmark:timing aborts: 'Required command not found: bc' (bc is a system package and root is unavailable)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
