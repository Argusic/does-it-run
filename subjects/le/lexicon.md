# Lexicon

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AashishH15/Lexicon, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/lexicon

## Pinned environment

- Project commit: `198a21c6428af41c292ea1eefd952ccc61d8350e`
- Test commit: `198a21c6428af41c292ea1eefd952ccc61d8350e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.3 to 3.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 3.3 | 2 | 2 | [run](https://argusic.com/run/5c17a0d1-5bcb-4546-b228-9cb5d43a9f0a) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `Node.js v18 is too old for Vite 7 (requires 20+). Frontend build failed with crypto.hash is not a function.`
- `Java JRE not installed; LanguageTool proofreading engine cannot start`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
