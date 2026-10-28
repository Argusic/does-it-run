# vector-storage

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nitaiaharoni1/vector-storage, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vector-storage

## Pinned environment

- Project commit: `0484d9c2576502192ee21989f09438817fd66207`
- Test commit: `0484d9c2576502192ee21989f09438817fd66207`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.5 to 10.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 10.5 | 3 | 3 | [run](https://argusic.com/run/0580b9a4-3368-4922-b5af-711d16bd3211) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `indexedDB is not defined in Node: library depends on browser IndexedDB via idb`
- 10 min: `Race: constructor kicked off async loadFromIndexDbStorage() unawaited, so addText/addTexts raced with the load and wiped documents`
- 8 min: `Hit counters never accumulated: updateHitCounters mutated result copies, not stored documents, breaking the documented LRU ordering`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
