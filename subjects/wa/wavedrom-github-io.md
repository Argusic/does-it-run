# wavedrom.github.io

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wavedrom/wavedrom.github.io, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/wavedrom-github-io

## Pinned environment

- Project commit: `41b69e34ca9ae54e3dcb4a88b71a3a79cbdf7724`
- Test commit: `41b69e34ca9ae54e3dcb4a88b71a3a79cbdf7724`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.6 to 25.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 25.6 | 2 | 2 | [run](https://argusic.com/run/37370c9c-20ce-44cf-a69c-6ffb437ac2e1) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `missing system zip/unzip binaries (no root); build's zip step failed silently so the .nw app package was never created`
- 15 min: `CLI PNG export broken (upstream bug): init.js pngdata() drew canvas before SVG Image loaded, produced empty data URL, wrote 3 garbage bytes instead of a PNG`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
