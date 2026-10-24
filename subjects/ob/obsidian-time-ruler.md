# obsidian-time-ruler

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/j-palindrome/obsidian-time-ruler, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/obsidian-time-ruler

## Pinned environment

- Project commit: `afbede327bc5a0591b26bf547638bc1b1e08fdfd`
- Test commit: `afbede327bc5a0591b26bf547638bc1b1e08fdfd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 3.3 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3 | 3.3 | 4 | 4 | [run](https://argusic.com/run/8a7c9148-e972-43bd-8acb-bf40250a0f66) |
| 2 | fail | 80 | 3 | 4.8 | 3 | 3 | [run](https://argusic.com/run/15da6aac-efea-4161-875f-25f78c4ae622) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not available in environment`
- 1 min: `tsconfig.json referred to vite/client type definitions that are not present (TS2688)`
- 1 min: `SettingsTab.tsx had unused 'import { log } from "console"' causing TS2307`
- `server directory included in root tsconfig caused TS errors for missing server deps`

Attempt 2:

- 1 min: `tsconfig.json references vite/client types not present in dependencies`
- 1 min: `TypeScript error: Type 'Timeout' not assignable to type 'number' in autoScroll.ts`
- 1 min: `Build script with VAULT env tries to mkdir //.obsidian/plugins (EACCES)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
