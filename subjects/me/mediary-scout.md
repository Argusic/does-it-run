# mediary-scout

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fancydirty/mediary-scout, licensed 0BSD, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mediary-scout

## Pinned environment

- Project commit: `eecbb42913255cadb9584af4f6040dbd64ed88f0`
- Test commit: `eecbb42913255cadb9584af4f6040dbd64ed88f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37.8 to 37.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 41 | 37.8 | 3 | 3 | [run](https://argusic.com/run/06c4ba50-94d2-403d-808a-9fe2ada6ff44) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `npm test could not resolve @media-track/workflow before its dist was built`
- 25 min: `Desktop dev launch: better-sqlite3 built for Node ABI 127, Electron 33 needs ABI 130 (bundled standalone copy)`
- 3 min: `System node is v18 but package.json requires >=22.13`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
