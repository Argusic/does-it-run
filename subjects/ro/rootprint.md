# rootprint

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rootprint/rootprint, licensed Apache-2.0, written in Svelte.

Evidence and recordings: https://argusic.com/subject/rootprint

## Pinned environment

- Project commit: `039450ec602e034e8569f6249dec01418ddd6f2e`
- Test commit: `039450ec602e034e8569f6249dec01418ddd6f2e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.6 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 14.6 | 4 | 4 | [run](https://argusic.com/run/9b45b460-3f6b-48bc-a284-f34650482991) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Bun not installed in container`
- 1 min: `Node.js v18.19.1 lacks node:util.styleText required by @sveltejs/kit and rolldown`
- 5 min: `No Docker - PostgreSQL and Quickwit unavailable`
- 2 min: `Quickwit on 0.0.0.0 unreachable via Bun's native fetch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
