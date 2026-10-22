# splicr

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Agions/splicr, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/splicr

## Pinned environment

- Project commit: `a33168b5e77c31376948fb8a4e4a0c3bae681d45`
- Test commit: `a33168b5e77c31376948fb8a4e4a0c3bae681d45`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28.2 to 28.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 24 | 28.2 | 3 | 2 | [run](https://argusic.com/run/16bfaf5a-c0ee-4453-b55c-e47c25fca3fb) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Base image lacked Rust toolchain, Node 22, and pnpm (corepack autopicked incompatible pnpm 12 and crashed)`
- 40 min: `Help page rendered '加载失败: [object Object]' in plain-browser/e2e mode because the useTauriQuery hook invoked Tauri IPC unconditionally and the fast-failing query hid the static shortcuts panel`
- 12 min: `Tauri desktop app binary cannot be built in this container: system dev libs glib-2.0/gio-2.0/gobject-2.0/gtk+-3.0/webkit2gtk-4.1/libsoup-3.0/sqlite3 .pc and headers are missing, no root or sudo to apt-install, and no bundled/prebuilt form e`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
