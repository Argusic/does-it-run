# elevenlabs-js

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elevenlabs/elevenlabs-js, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/elevenlabs-js

## Pinned environment

- Project commit: `b6deef08ed7c65134176482af69ceb4d348e1817`
- Test commit: `b6deef08ed7c65134176482af69ceb4d348e1817`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 19.3 to 95.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 2 | 95.1 | 3 | 3 | [run](https://argusic.com/run/9f356638-4e50-4df3-9c18-ac46e43b1616) |
| 2 | pass with mocks | 92 | 4 | 19.3 | 5 | 5 | [run](https://argusic.com/run/b9913229-19c4-4cf9-9217-f0b5d6706c5f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `yarn binary unavailable (no root for global install), npm install used instead`
- 8 min: `3 unit tests failed on Node 18.19.1: ReferenceError: File is not defined`
- 20 min: `15 custom integration tests failed with HTTP 401 Invalid API key against api.elevenlabs.io`

Attempt 2:

- 5 min: `Node 18 lacks global File API (project requires Node 20+ per CONTRIBUTING), causing 3 fetcher unit tests to crash with 'File is not defined'`
- 45 min: `15 custom live-API tests in tests/custom/client.test.ts fail without an ElevenLabs API key`
- 6 min: `npm package entry index.js does not exist in the repo (produced only by prepack); probe originally imported ../../index.js and hit ERR_MODULE_NOT_FOUND`
- 8 min: `Initial mock's dummy mp3 bytes are not a decodable mp3; ffmpeg decode of generated audio failed`
- 2 min: `mpv is not installed in the container, so the stream() helper check could not exercise playback`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
