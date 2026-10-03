# Archon

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coleam00/Archon, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/archon

## Pinned environment

- Project commit: `4d48a0325e64017aaaf2b3ad21c0faf9dc368520`
- Test commit: `4d48a0325e64017aaaf2b3ad21c0faf9dc368520`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services, real run
- Valid runs: 3; wall time 33.4 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/fd1a7b91-1a97-47a4-8cb4-7d85d6985bae) |
| 2 | pass with mocks | 92 | 3.2 | 33.4 | 2 | 2 | [run](https://argusic.com/run/5a3eee0f-e07b-4af8-bab5-e204f053565a) |
| 3 | pass | 100 | 34 | 36.4 | 3 | 3 | [run](https://argusic.com/run/6b65b2a1-2ce6-4ad1-ad99-114247cc218e) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `unzip not available, bun.sh installer failed`
- 1.5 min: `Node.js v18.19.1 too old for @archon/docs-web package (needs >=22.12.0)`

Attempt 3:

- 2 min: `Bun runtime was not installed in the container`
- 3 min: `CLI test failure: import boundary expectations stale for bun 1.4.2's code-split chunk grouping`
- 1 min: `Server dev mode crashed with EMFILE from Bun file watcher (container file-descriptor limit)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
