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
- Valid runs: 2; wall time 4.8 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 13 | 7 | 7 | [run](https://argusic.com/run/08b6d16a-b616-4af9-a74c-1363ef02b047) |
| 2 | pass | 100 | 5 | 4.8 | 6 | 6 | [run](https://argusic.com/run/c8a11672-b872-451c-9155-d955f653ccfe) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed`
- 2 min: `Node 18 too old (requires >=22)`
- 2 min: `Rust not found`
- 1 min: `pnpm build approvals required`
- 3 min: `glib-2.0.pc missing (Tauri dep)`
- 3 min: `gobject-2.0/gio-2.0 .pc files chain`
- 1 min: `gdk-sys (GTK3 dev) not buildable`

Attempt 2:

- 2 min: `Node.js v18 too old (requires >=22)`
- 1 min: `pnpm not installed`
- 2 min: `Rust not installed`
- 1 min: `pnpm install blocked on esbuild/sharp build scripts`
- 0.5 min: `CLI collection missing .apiark/apiark.yaml config`
- 0.5 min: `CLI config version field type mismatch (string vs u32)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
