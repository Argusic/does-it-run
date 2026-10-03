# illa-builder

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/illacloud/illa-builder, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/illa-builder

## Pinned environment

- Project commit: `a468660903e2a17b1778ba97dd17a375181a72e0`
- Test commit: `a468660903e2a17b1778ba97dd17a375181a72e0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 6.4 to 13.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 6 | 6.4 | 3 | 3 | [run](https://argusic.com/run/ed9ed259-3aac-4403-8170-2ceac708ff42) |
| 2 | fail | 80 | 3 | 13.3 | 7 | 7 | [run](https://argusic.com/run/1dd1515c-6eaf-4199-aa12-d16880937121) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm not found in PATH (only npm v9 was available)`
- 1 min: `Git submodules (illa-design, illa-public-component) were empty, causing ERR_PNPM_WORKSPACE_PKG_NOT_FOUND`
- `No test tasks defined in any workspace package.json - 'turbo run test' fails`

Attempt 2:

- 1 min: `pnpm lockfileVersion 6.0 incompatible with pnpm 12.x`
- 1 min: `pnpm blocks build scripts by default`
- 1 min: `Missing locale files at apps/builder/src/i18n/locale/`
- 1 min: `@uiw/codemirror-theme-github/src subpath import not resolved`
- 1 min: `chroma-js@2.6.0 does not export named 'hsv'`
- 1 min: `Pre-existing TypeScript errors in submodules`
- 2 min: `OOM (exit 137) during chunk rendering`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
