# TalkingHead

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/met4citizen/TalkingHead, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/talkinghead

## Pinned environment

- Project commit: `b3e277b3b46f88e557bf28a2c5612a5b04e075c3`
- Test commit: `b3e277b3b46f88e557bf28a2c5612a5b04e075c3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.8 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 13.8 | 4 | 4 | [run](https://argusic.com/run/4d5be63d-53d6-4765-96b1-10e025e5c9b6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Puppeteer v24 requires Node >=20 (container has v18.19.1)`
- 2 min: `Remote avatar URL (models.readyplayer.me) unreachable from container`
- 1 min: `Import map in test HTML used CDN URLs for three.js`
- 1 min: `Avatar path was relative to test dir causing 404`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
