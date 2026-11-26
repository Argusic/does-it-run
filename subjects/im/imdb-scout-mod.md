# IMDb-Scout-Mod

**Verdict: runs with mocks.** Argusic Score 90.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Purfview/IMDb-Scout-Mod, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/imdb-scout-mod

## Pinned environment

- Project commit: `07d0ff2c9c14a45e4f26cbc18046c1175da42f4c`
- Test commit: `07d0ff2c9c14a45e4f26cbc18046c1175da42f4c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 16.9 to 47 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88.67 | 30 | 47 | 6 | 5 | [run](https://argusic.com/run/ffac102d-5c5e-4b08-9350-95fa3d4a6848) |
| 2 | pass with mocks | 92 | 4 | 16.9 | 4 | 4 | [run](https://argusic.com/run/72a95c17-d81e-467a-95e3-3e7cfa5d6fa8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `jsdom lacks structuredClone which the script uses`
- 3 min: `GM_config failed to initialize without GM_getValue/GM_setValue or localStorage`
- 2 min: `Top-level 'return;' statements are illegal when the script body is wrapped for Node vm eval`
- 4 min: `Fixture lacked .ipc-page-section--sp-pageMargin so getLinkArea() could not insert the header and iconSorterFound threw on null`
- 1 min: `External rating hosts (Letterboxd/OMDb/Metacritic) unreachable from the container`
- 10 min: `No browser/Tampermonkey/Greasemonkey installed and no root to install system packages, so a real Greasy Fork browser install cannot be exercised`

Attempt 2:

- 2 min: `Chrome headless browser not available in container`
- 1 min: `Required userscript runtime dependencies (jQuery, GM_config, ExEv, gm4-polyfill) not present`
- 1 min: `Anti-bot gokuProps check false-positive when script source is embedded in page DOM (test environment only; not an issue in real Tampermonkey/Violentmonkey sandbox)`
- 2 min: `Top-level 'return' statement at line 11650 causes 'Illegal return statement' when loaded via <script> tag (valid in userscript manager's async wrapper)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
