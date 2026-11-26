# steam-achievement-manager-windows

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/solv4626/steam-achievement-manager-windows, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/steam-achievement-manager-windows

## Pinned environment

- Project commit: `fe595575cf64d085479141931d28e357a7327f19`
- Test commit: `fe595575cf64d085479141931d28e357a7327f19`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 4.2 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.5 | 4.2 | 3 | 3 | [run](https://argusic.com/run/15bd1068-6dcc-4326-a085-50d7493fa30c) |
| 2 | fail | 80 | 18 | 11.5 | 3 | 3 | [run](https://argusic.com/run/c0a693b2-0da6-4055-a1a2-3adedcafa7b5) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Rust toolchain (rustc, cargo) not installed in container`
- 0.5 min: `GUI/adwaita build fails: missing glib-2.0.pc, gtk4.pc, libadwaita-1.pc dev packages`
- `10 integration tests fail: require running Steam client with Steam data files`

Attempt 2:

- 14 min: `GTK4/Adwaita -dev packages (.pc files, headers) not installed in container (no root access)`
- 0.5 min: `glib-compile-schemas not on default PATH`
- `msgfmt (gettext) not available for translations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
