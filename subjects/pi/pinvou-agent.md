# pinvou-agent

**Verdict: runs.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Pinvou/pinvou-agent, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/pinvou-agent

## Pinned environment

- Project commit: `b7a814bc8b90987fff4443fc265fb36e3a435749`
- Test commit: `b7a814bc8b90987fff4443fc265fb36e3a435749`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 26.8 to 40.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 18 | 26.8 | 2 | 0 | [run](https://argusic.com/run/c73a5e4c-85fa-4c46-8861-2e21f5050dbf) |
| 2 | fail | 20 | 38 | 40.9 | 6 | 6 | [run](https://argusic.com/run/310076d6-a7ec-4141-a0f0-201d73789f5c) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Tauri Rust backend cannot build: missing webkit2gtk-4.1, libsoup-3.0, glib-2.0 system dev packages (no root access)`
- 2 min: `npm run lint:ui fails: ESLint 10 incompatibility with typescript-eslint plugin (TypeError: mapTypes.union is not a function)`

Attempt 2:

- `npm ci , EBADENGINE warnings for yargs requiring node >=20, but npm installed 603 packages without failure`
- 3 min: `Node.js v18.19.1 too old , Vite 8/rolldown needs node:util.styleText (Node >=20)`
- 1 min: `rolldown native binding missing , optional @rolldown/binding-linux-x64-gnu not installed by npm ci`
- 1 min: `vite build succeeds, then Tauri build fails , missing SenseVoice runtime dependency (file command not installed)`
- 5 min: `Tauri Rust build fails , missing system dev libraries: webkit2gtk-4.1, libsoup-3.0, glib-2.0-dev, gtk-3-dev, and their transitive .pc files`
- `TypeScript check shows 10+ implicit-any type errors in JSX files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
