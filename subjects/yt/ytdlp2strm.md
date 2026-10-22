# ytdlp2STRM

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fe80Grau/ytdlp2STRM, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ytdlp2strm

## Pinned environment

- Project commit: `bcc67af191dd2d09d54a4da4228a49789f346fbe`
- Test commit: `bcc67af191dd2d09d54a4da4228a49789f346fbe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 5.3 to 9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 5.3 | 0 | 0 | [run](https://argusic.com/run/66703914-330c-4dad-954c-5cab7f191afe) |
| 2 | pass | 100 | 0.5 | 9 | 3 | 3 | [run](https://argusic.com/run/75dc9a6a-ef0b-496d-876c-1552758c6be1) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `CLI '--version' argument defined without 'action='store_true'', causing argparse error 'expected one argument'`
- `yt-dlp binary not on system PATH (only in venv/bin/)`
- `Plugins (YouTube/Twitch) find no videos in container without browser cookies`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
