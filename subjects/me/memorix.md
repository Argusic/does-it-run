# memorix

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AVIDS2/memorix, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/memorix

## Pinned environment

- Project commit: `e23eca9b295c9a24b67b5abd47ae46f1a7137dd1`
- Test commit: `e23eca9b295c9a24b67b5abd47ae46f1a7137dd1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.6 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.6 | 3 | 3 | [run](https://argusic.com/run/60da4e0d-0d74-43aa-873f-e30ae7b2391d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node is v18.19.1 but project requires >=22.18.0`
- 2 min: `Manual JSON-RPC initialize on MCP stdio closed stdin before server responded`
- 2 min: `Initial invocation of smoke-stateless-http.mjs via sh hung`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
