# mygo

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/egoist/mygo, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/mygo

## Pinned environment

- Project commit: `b0604652c0e9e84550ebf6c7e5bfbb359b32e050`
- Test commit: `b0604652c0e9e84550ebf6c7e5bfbb359b32e050`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 11.1 to 21.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.3 | 11.1 | 2 | 2 | [run](https://argusic.com/run/9af2bfce-9363-4732-9130-f9032e60aff5) |
| 2 | fail | 20 | n/a | 21.7 | 0 | 0 | [run](https://argusic.com/run/b9313d95-bbc0-4919-af3b-9ba450b7ec29) |

## What was observed on a clean machine

Attempt 1:

- `No GPU render node (/dev/dri/renderD*): AST display-only DRM driver, no 3D`
- `WebKitGTK (libwebkit2gtk-4.1.so.0) not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
