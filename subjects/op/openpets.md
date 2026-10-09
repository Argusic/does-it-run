# openpets

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenPetsHQ/openpets, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openpets

## Pinned environment

- Project commit: `2d14120cf027c9e80db7ff78e60711be08d39df4`
- Test commit: `2d14120cf027c9e80db7ff78e60711be08d39df4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 58.2 to 58.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 58.2 | 4 | 4 | [run](https://argusic.com/run/c170ee32-669f-4c4b-a2f2-2bf1e7a38502) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 does not satisfy the >=20 engine requirement`
- 1 min: `openpets.system-resources git submodule not initialized`
- 3 min: `rpmbuild not available in test container for packaging fixture tests`
- 20 min: `voice-media-player.test.ts fails on Node.js 22 strict unhandled rejection mode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
