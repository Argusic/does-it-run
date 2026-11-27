# 33-js-concepts

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leonardomso/33-js-concepts, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/33-js-concepts

## Pinned environment

- Project commit: `16d0d95c02b19df6a8c841f1a0012d7b7367a340`
- Test commit: `16d0d95c02b19df6a8c841f1a0012d7b7367a340`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.05 | 7.8 | 6 | 6 | [run](https://argusic.com/run/e48e2ac6-2954-4ee0-8727-737d86014160) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `vitest 4.x requires Node 20+ (styleText export); Node 18 in container`
- 2 min: `ES2023+ features missing in Node 18 (Array.prototype.toSorted/toReversed/toSpliced, Object.groupBy)`
- 1 min: `File and CustomEvent constructors not available in Node 18`
- 3 min: `WeakMap/WeakSet Symbol keys not supported in Node 18 V8`
- 1 min: `URL.createObjectURL not implemented in jsdom 24`
- 2 min: `Node 18 native FormData returns internal File type without preserving custom File.name property`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
