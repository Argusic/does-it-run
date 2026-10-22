# node-sonos

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bencevans/node-sonos, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/node-sonos

## Pinned environment

- Project commit: `ceaa85502d4953cdec472d42664ffaf939a4104f`
- Test commit: `ceaa85502d4953cdec472d42664ffaf939a4104f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25.8 to 25.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 26 | 25.8 | 1 | 1 | [run](https://argusic.com/run/ec233d64-6420-4d06-96ee-0283d6ba45a1) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `Mock SOAP responses were malformed (double closing tags, over-escaped TrackMetaData, literal ZoneGroupState wrapper, SSDP bound only to 127.0.0.1)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
