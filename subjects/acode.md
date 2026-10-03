# Acode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Acode-Foundation/Acode, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/acode

## Pinned environment

- Project commit: `b7dbe3d69dcf5165e19581fe3927f0838dce09f4`
- Test commit: `b7dbe3d69dcf5165e19581fe3927f0838dce09f4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.6 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 13.6 | 6 | 6 | [run](https://argusic.com/run/f12291ec-ba07-4e6f-9bd1-af099631ebd1) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `codemirror-lsp-client submodule was empty; npm install failed because its prepare script (cm-buildhelper) ran before its own devDependencies were installed`
- 5 min: `Node 18 lacks node:util.styleText used by vitest v4/rolldown`
- 1 min: `npm install with Node 22 hit arborist bug on package-lock.json from Node 18`
- 1 min: `6 tests in lspMultiClient.test.js failed: multiple instances of @codemirror/state loaded, breaking instanceof checks`
- 1 min: `immersiveFullscreenPrepare.test.js timed out after 5s formatting a 23KB Java file with prettier-plugin-java`
- `cordova build/android launch failed (no JDK/Android SDK)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
