# LittleJS

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KilledByAPixel/LittleJS, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/littlejs

## Pinned environment

- Project commit: `ba5064e0355f300128b9ab4b88cf6a284cf67894`
- Test commit: `ba5064e0355f300128b9ab4b88cf6a284cf67894`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 40.8 to 40.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.25 | 40.8 | 5 | 5 | [run](https://argusic.com/run/cbd77144-e7cd-4fdb-aa01-4bbde9c63bd5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18.19.1 is below required ^20.19.0 , ESM import of dist/littlejs.esm.js fails without "type":"module" in package.json`
- 9 min: `With "type":"module", require() on CJS box2d.wasm.js triggers ERR_REQUIRE_ESM in all 7 box2d test files`
- 5 min: `Node 18 ESM mode has no global crypto object , newgrounds tests fail at ASSERT and crypto.subtle.encrypt is undefined`
- 2 min: `performance.now is read-only on Performance.prototype in Node 18 , r5d-inputaudio test throws on assignment`
- 1 min: `util.test.mjs shareURL test needs navigator global , crashes with ReferenceError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
