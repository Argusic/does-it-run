# NASSAV

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Satoing/NASSAV, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/nassav

## Pinned environment

- Project commit: `0c5ff7fe11d77cae5d4367776bce92e1b687c6ae`
- Test commit: `0c5ff7fe11d77cae5d4367776bce92e1b687c6ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 6.5 to 17 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 6.5 | 0 | 0 | [run](https://argusic.com/run/36fe792e-169b-42e9-aff0-0b2df0f56e21) |
| 2 | pass with mocks | 92 | 18 | 17 | 7 | 7 | [run](https://argusic.com/run/441e9117-56fd-43ca-8121-867a88425b57) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `go binary not installed and no root to apt-install it (README requires Go 1.22.6)`
- 25 min: `curl_cffi ignores SSL_CERT_FILE and no /etc/hosts write access, so real hostnames (memojav.com, www.javbus.com) could not be pointed at the local mock`
- 3 min: `mock's Memo get_video_info returned a raw URL but MemoDownloader.parseHTML expects percent-encoded https%3A%2F%2F URL`
- 8 min: `m3u8-Downloader-Go download failed against the mock: tls: certificate signed by unknown authority with proxy, then 404 without proxy`
- 10 min: `scraper cover image fetch returned HTTP 405 Method Not Allowed through the proxy`
- 2 min: `relative fanart sample URLs in the JavBus mock page failed with 'URL rejected: No host part' (app does not absolutize relative URLs)`
- 2 min: `backend/main.go hardcodes basePath /vol2/1000/MissAV which is not writable in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
