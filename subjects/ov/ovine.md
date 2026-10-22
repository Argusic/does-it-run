# ovine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ovineio/ovine, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ovine

## Pinned environment

- Project commit: `cb2d4f98946509cc0e0ca8ce4db97e524f9583b6`
- Test commit: `cb2d4f98946509cc0e0ca8ce4db97e524f9583b6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.7 to 15.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 15.7 | 3 | 3 | [run](https://argusic.com/run/ee67bc89-c291-4195-b97f-f1d10c7db048) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `yarn.lock had 2 packages pinned to unreachable Chinese mirror registry.nlark.com`
- 1 min: `CLI binary failed to start because tsc didn't copy webpack plugin .js files to lib/`
- 2 min: `ttypescript/ttsc has a compatibility crash with Node.js 18 (extends/getter issue)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
