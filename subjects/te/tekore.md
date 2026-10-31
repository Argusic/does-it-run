# tekore

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/felix-hilden/tekore, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tekore

## Pinned environment

- Project commit: `2438a90a5fb2157b805814d5cb7aca920883ed86`
- Test commit: `2438a90a5fb2157b805814d5cb7aca920883ed86`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.6 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 11 | 13.6 | 7 | 7 | [run](https://argusic.com/run/dee963a4-49e3-4a1b-be21-2991478c5540) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `mock server reaped between tool calls (connection refused)`
- 1 min: `mock rejected Basic auth: 400 invalid_client`
- 1 min: `mock returned incomplete FullAlbum schema (6 pydantic validation errors)`
- 1 min: `UnknownModelAttributeWarning on album tracks (SimpleTrack rejects album/external_ids/popularity)`
- 1 min: `404 for playback_currently_playing (path /v1/me/player/currently-playing)`
- 1 min: `ConversionError: playback_start_tracks rejected 'spotify:track:t1'`
- 1 min: `TypeError: request_client_token got unexpected 'asynchronous' kwarg`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
