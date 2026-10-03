# Yoopta-Editor

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yoopta-editor/Yoopta-Editor, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/yoopta-editor

## Pinned environment

- Project commit: `070349b1cd703d05548e2db94c98b4e9622d4f07`
- Test commit: `070349b1cd703d05548e2db94c98b4e9622d4f07`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.2 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 1 | 20.2 | 2 | 1 | [run](https://argusic.com/run/8e4b49c6-bd8b-4c23-aa18-1c1f0d0b776f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18.19.1 bundled in container is too old: yarn 4.12.0 works but some packages need newer Node (next-app-example requires >=20.9.0; vitest v4 requires >=22). Builds failed intermittently with signal 129 (SIGHUP) at default turbo concu`
- `1 pre-existing test failure: packages/core/collaboration/src/with-collaboration.test.ts:232 - 'should auto-connect when connect is not false'. Implementation uses strict equality (config.connect === true) but test expects truthiness (connec`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
