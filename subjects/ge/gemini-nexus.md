# Gemini-Nexus

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yeahhe365/Gemini-Nexus, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/gemini-nexus

## Pinned environment

- Project commit: `aeaa06cce02dcd6502215600f0c123a7e6c0ac44`
- Test commit: `aeaa06cce02dcd6502215600f0c123a7e6c0ac44`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.8 to 12.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 12.8 | 2 | 2 | [run](https://argusic.com/run/6d4c1f5f-348b-406f-a7da-a82164de403c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `jsdom@27.0.1 requires Node >=20; SharedArrayBuffer.prototype.growable is undefined in Node 18, causing webidl-conversions to crash and 4 content/ test files (speech_reader, youtube_summary, toolbar/events, toolbar/templates) to fail`
- 3 min: `knip@6.13.1 requires Node >=20; styleText is not exported from node:util in Node 18, causing the lint:unused (knip) step to crash`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
