# dsh-purge

**Verdict: runs with mocks.** Argusic Score 46 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kingcharleslzy-ai/dsh-purge, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/89c1e2dd-c7ab-4615-b4bb-967ae43c179f

## Pinned environment

- Project commit: `27919a326b6615b1968661a3e749760cec3a2e07`
- Test commit: `27919a326b6615b1968661a3e749760cec3a2e07`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 1 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 7 | 4 | 4 | [run](https://argusic.com/run/89c1e2dd-c7ab-4615-b4bb-967ae43c179f) |
| 2 | fail | 0 | 5 | 1 | 2 | 0 | [run](https://argusic.com/run/8dcf230e-e8f1-4f62-90a5-ad3ea7dc4501) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18.19.1 lacks import.meta.dirname; test/no-region-gate.test.mjs threw TypeError`
- 3 min: `18 failures in test/steering-runtime.test.mjs (native/upstream/negative-control steering runtime) on Node 18`
- 1 min: `test/redteam-host.test.mjs drill-tool test fails: node:sqlite is a Node 22-only builtin, absent on Node 18`
- 6 min: `Community installer real run initially failed because my mock DSH CLI unpacked the tgz into profile node_modules root instead of node_modules/dsh-purge-community and exited before async add completed`

Attempt 2:

- 5 min: `Repository is an AI safety-circumvention toolkit (removes sandboxing, approvals, and model refusal behavior); declined to install or verify it.`
- `No DSH host/CLI exists in the container, which the installer requires.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
