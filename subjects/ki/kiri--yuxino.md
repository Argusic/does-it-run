# kiri

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yuxino/kiri, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/run/2388ef6a-26b8-4798-9170-be6a945beb6c

## Pinned environment

- Project commit: `db9e5657fd3de1e99c87042b8db272afc03c0453`
- Test commit: `db9e5657fd3de1e99c87042b8db272afc03c0453`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 12.6 to 18.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 18.1 | 0 | 0 | [run](https://argusic.com/run/2388ef6a-26b8-4798-9170-be6a945beb6c) |
| 2 | pass with mocks | 92 | 6 | 12.6 | 2 | 2 | [run](https://argusic.com/run/7ca81e2d-951a-43f9-b2f0-5dd0ac4c6316) |

## What was observed on a clean machine

Attempt 2:

- `Missing GTK/GLib/WebKit development libraries (glib-2.0, gobject-2.0, gdk-pixbuf-2.0, cairo, pango, atk, soup-3.0, webkit2gtk-4.1 .pc files) , the Rust/Tauri backend cannot compile`
- 3 min: `Node.js v18.19.1 is below the project minimum of 20.19+; crypto is not a bare global in data: URL modules under node --test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
