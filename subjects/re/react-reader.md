# react-reader

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gerhardsletten/react-reader, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-reader

## Pinned environment

- Project commit: `70d489366b3b57d89b9a9da7b104c261279d9ca6`
- Test commit: `70d489366b3b57d89b9a9da7b104c261279d9ca6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.6 to 11.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10.8 | 11.6 | 5 | 5 | [run](https://argusic.com/run/8ae6372b-410e-43c9-8d92-255b5cae8d6d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm test exited 1: No tests found - the repo ships zero test files`
- 1 min: `Test TS errors: verbatimModuleSyntax from root tsconfig leaked into test compile; @testing-library/user-event not installed; matcher types not loaded`
- 1 min: `Test UX bugs in my new tests (undefined button, wrong EpubView assertion, mock typing)`
- 1 min: `Demo smoke: vite preview served 404 after library build clobbered the demo dist`
- `unzip/headless browser not installed in container; xdg-open missing so vite dev/preview print a harmless open-error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
