# parse-video

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wujunwei928/parse-video, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/parse-video

## Pinned environment

- Project commit: `57590df94b49aafc827eb98e85c845eaa1cb3daf`
- Test commit: `57590df94b49aafc827eb98e85c845eaa1cb3daf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.7 to 19.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 58 | 19.7 | 3 | 3 | [run](https://argusic.com/run/e3713b40-8e64-405c-a972-0320f6ade356) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain absent in container (go: not found); installed user-local Go 1.24.0 and built the project`
- 5 min: `Running 'go run main.go' with default rate limit hit 429 on every non-exempt API request, blocking first-request verification`
- 20 min: `Real douyin and bilibili parses failed against live platforms: real douyin page no longer embeds detail (PARSE_VIDEO_DOUYIN_COOKIE required), douyin web detail API returned 403 ArgusSecurityPlugin, bilibili view API returned 412 request ban`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
