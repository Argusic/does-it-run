# comics-downloader

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Girbons/comics-downloader, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/comics-downloader

## Pinned environment

- Project commit: `e71c68c43eb43a01198b4c9bc8d5b01a3184c456`
- Test commit: `e71c68c43eb43a01198b4c9bc8d5b01a3184c456`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 74.4 to 74.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 76 | 74.4 | 5 | 5 | [run](https://argusic.com/run/f32fe1e1-9785-409a-b91c-b74880a000c6) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `go toolchain missing in container`
- 6 min: `go build failed: github.com/nwaples/rardecode/v2 v2.2.0 lacks WriteTo required by mholt/archives`
- 10 min: `mangatown image host zjcdn.mangahere.org returned 403 without Referer, producing empty PDF/CBZ files`
- 4 min: `cmd/gui cannot build: missing X11/Xlib.h, libGL pkg-config, and GLFW headers (no root to install system packages)`
- 22 min: `legacy tests fail because comicextra.me now serves a JS-gated page with zero comic links (tests assert 23) and mangakakalot domain redirects to a placeholder, causing a nil-pointer panic in MangaKakalotInitialize`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
