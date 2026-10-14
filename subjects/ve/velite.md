# velite

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zce/velite, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/velite

## Pinned environment

- Project commit: `04453e39df0ffee661474e981355e2e3b4e63867`
- Test commit: `04453e39df0ffee661474e981355e2e3b4e63867`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11 to 11 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 11 | 3 | 3 | [run](https://argusic.com/run/763d0c9d-57da-424c-bb54-e972b95f4bfe) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `pnpm not installed; global npm prefix /usr/local is root-owned (no root in container)`
- 12 min: `Container Node is v18.19.1; project engines require ^18.20||>=20.3, and Next.js/Vite fixture tests fail with 'CustomEvent is not defined' because Vite 8 requires Node >=20.19`
- 8 min: `Initial pnpm install under Node 18 skipped rolldown's optional native binding '@rolldown/binding-linux-x64-gnu' (its engines exclude Node 18), so Vite fixture crashed with MODULE_NOT_FOUND for rolldown-binding.linux-x64-gnu.node`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
