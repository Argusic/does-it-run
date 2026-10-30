# tiptap-ui-components

**Verdict: could not verify.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ueberdosis/tiptap-ui-components, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tiptap-ui-components

## Pinned environment

- Project commit: `799929bea4804c73767562b69f8acc2acdb8ac86`
- Test commit: `799929bea4804c73767562b69f8acc2acdb8ac86`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 2.2 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 70 | 0.1 | 3.9 | 2 | 1 | [run](https://argusic.com/run/e5080db5-d042-4140-9994-1805d27613d0) |
| 2 | fail | 80 | 0.5 | 2.2 | 2 | 2 | [run](https://argusic.com/run/97bb6a3b-0c14-44ef-b7d3-2b88977b5afe) |

## What was observed on a clean machine

Attempt 1:

- 0.6 min: `pnpm 9.0.0 not found in PATH`
- `eslint rule 'react-hooks/exhaustive-deps' not found (pre-existing lint config gap)`

Attempt 2:

- 0.5 min: `pnpm not installed globally (Node v18 has no corepack)`
- `tiptap info fails: Failed to load jsconfig.json. Couldn't find tsconfig.json`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
