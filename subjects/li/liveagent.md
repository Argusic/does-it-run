# LiveAgent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Stack-Cairn/LiveAgent, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/liveagent

## Pinned environment

- Project commit: `a41515366d7ea1bde7aaefe57ba38c24f6210389`
- Test commit: `a41515366d7ea1bde7aaefe57ba38c24f6210389`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 32.4 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/ef4f74f6-d22a-43f7-b18f-ef161ed06f44) |
| 2 | pass | 100 | 28 | 32.4 | 7 | 7 | [run](https://argusic.com/run/1b327766-c87a-4562-8d76-d3943be6c9aa) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js 18.19.1 is too old for Vite 8 (requires 20.19+ or 22.12+)`
- 2 min: `pnpm not available on system PATH`
- 1 min: `Native binding @rolldown/binding-linux-x64-gnu missing after first pnpm install`
- 10 min: `Vite build (pnpm build:gui and pnpm build:webui) OOM killed (exit 137) on 2GB container during rolldown chunking`
- 3 min: `Rust cargo check fails: missing system library gobject-2.0 (gobject-sys crate) , Tauri/WebKit dependency`
- 1 min: `Go gateway build requires web/dist for embedded assets , not built due to Vite OOM`
- 1 min: `TestTunnelTrafficWhileControlPlaneBusy flaky (7 < 10 requests in 2s on constrained container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
