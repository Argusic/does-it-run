# plano

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/katanemo/plano, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/plano

## Pinned environment

- Project commit: `003c36aea896ce6fa98567329588baa582e41f9c`
- Test commit: `003c36aea896ce6fa98567329588baa582e41f9c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 20.9 to 35.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 20.9 | 0 | 0 | [run](https://argusic.com/run/423bce33-ff43-4883-9693-5a65fc4cbd94) |
| 2 | pass | 100 | 5 | 35.9 | 4 | 4 | [run](https://argusic.com/run/116ae4c9-5338-48ea-9c11-97bf9f111ff5) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `uv build fails: hatchling 'Forced include not found: ../config/envoy.template.yaml' in the build sandbox`
- 2 min: `Editable/source CLI installs lack planoai/data config templates, so 'planoai up' outside the repo fails with 'Could not find config templates'`
- 1 min: `Non-SSE mock upstream with stream=true yields HTTP 200 empty body because the wasm llm_gateway buffers incomplete SSE`
- `Mock helper processes died when the parent shell exited`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
