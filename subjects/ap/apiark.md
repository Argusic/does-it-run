# apiark

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/berbicanes/apiark, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/apiark

## Pinned environment

- Project commit: `46ba45acdc921bcf828c61190d8143e73525fd40`
- Test commit: `46ba45acdc921bcf828c61190d8143e73525fd40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 13 | 7 | 7 | [run](https://argusic.com/run/08b6d16a-b616-4af9-a74c-1363ef02b047) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed`
- 2 min: `Node 18 too old (requires >=22)`
- 2 min: `Rust not found`
- 1 min: `pnpm build approvals required`
- 3 min: `glib-2.0.pc missing (Tauri dep)`
- 3 min: `gobject-2.0/gio-2.0 .pc files chain`
- 1 min: `gdk-sys (GTK3 dev) not buildable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
