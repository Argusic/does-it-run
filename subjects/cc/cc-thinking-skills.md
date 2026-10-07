# cc-thinking-skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tjboudreaux/cc-thinking-skills, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/cc-thinking-skills

## Pinned environment

- Project commit: `7b8fece345dfaa11773be7152ccd194589cb5437`
- Test commit: `7b8fece345dfaa11773be7152ccd194589cb5437`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.8 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0 | 5.8 | 2 | 2 | [run](https://argusic.com/run/7f38b63b-316e-4776-8e58-1e8983df39ff) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `evidence-registry-generation.test.js: 2 tests failed because 3 git SHAs (c2e4a73, 3d1f67d, 1d63b0d) not in shallow clone`
- `ambiguous ref warning from earlier git fetch creating a 40-hex ref`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
