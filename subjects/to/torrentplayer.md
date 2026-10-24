# torrentplayer

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/torrentplayer/torrentplayer, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/torrentplayer

## Pinned environment

- Project commit: `75b7bcaf9ba36c712e772773b0e49333710f29e1`
- Test commit: `75b7bcaf9ba36c712e772773b0e49333710f29e1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 15.9 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 18.7 | 0 | 0 | [run](https://argusic.com/run/f5f51ee3-8310-422d-a66c-10e10a8b194b) |
| 2 | pass | 100 | 12 | 15.9 | 1 | 1 | [run](https://argusic.com/run/3717572b-cb8d-41e2-bb33-f38eedce1139) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `Tauri GUI (src-tauri) build fails: missing system GTK/WebKitGTK -dev packages (libwebkit2gtk-4.1-dev, libgtk-3-dev, libjavascriptcoregtk-4.1-dev, libcairo2-dev, libpango1.0-dev, libsoup-3.0-dev, zlib1g-dev, libharfbuzz-dev, libfreetype, lib`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
