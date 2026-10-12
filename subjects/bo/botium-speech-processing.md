# botium-speech-processing

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/codeforequity-at/botium-speech-processing, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/botium-speech-processing

## Pinned environment

- Project commit: `33db7c08d24daa4087649975422cd73700bc5ffc`
- Test commit: `33db7c08d24daa4087649975422cd73700bc5ffc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 5.9 | 5 | 5 | [run](https://argusic.com/run/2642be0c-0b2b-4052-98d1-f43f9b6a2ad2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 installed but engine requires >=20`
- 1 min: `Uncommenting commented-out engines in routes.js introduced missing comma syntax error`
- 5 min: `Default backends (MaryTTS, Kaldi) unreachable without Docker`
- `sox/soxi not installed , cannot install system packages without root`
- `pico2wave not installed , svox-pico-tts system package not available without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
