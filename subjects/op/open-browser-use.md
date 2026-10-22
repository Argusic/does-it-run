# open-browser-use

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iFurySt/open-browser-use, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/open-browser-use

## Pinned environment

- Project commit: `1489c22e357a1b73b649b7a4061cc91d6d8dc03e`
- Test commit: `1489c22e357a1b73b649b7a4061cc91d6d8dc03e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.2 to 13.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 13.2 | 3 | 3 | [run](https://argusic.com/run/4fe47b29-7695-452a-88e6-989cc6b170fa) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Node 18 ESM: globalThis.crypto is undefined, so webmcp.test.mjs failed 2 tests (crypto.randomUUID() in sandboxed background.js getInfo)`
- 5 min: `go, pnpm, and pytest not preinstalled; npm global install blocked by EACCES on /usr/local (no root)`
- 1 min: `obu setup without --external-extension-output fails: cannot mkdir /opt/google/chrome/extensions (permission denied)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
