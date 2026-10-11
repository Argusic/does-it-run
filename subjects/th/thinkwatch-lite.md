# ThinkWatch-Lite

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ThinkWatchProject/ThinkWatch-Lite, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/thinkwatch-lite

## Pinned environment

- Project commit: `d1742e99091f00b82d803d40ae49102ae5c0dccf`
- Test commit: `d1742e99091f00b82d803d40ae49102ae5c0dccf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 7.8 | 5 | 5 | [run](https://argusic.com/run/0a85fa7c-44e0-4999-8038-dd73b3a25153) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm v11.13.0 is a broken release and cannot be installed`
- 1 min: `npm EACCES permission denied installing global pnpm`
- 1 min: `Node.js v18.19.1 too old for Vite 7 (needs 20.19+)`
- 2 min: `@tailwindcss/oxide native binding missing after pnpm install`
- `Rust main crate requires system dev packages (glib2, gtk3, webkit2gtk, libsoup) not available without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
