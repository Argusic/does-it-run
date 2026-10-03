# wacrm

**Verdict: runs with mocks.** Argusic Score 84 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ArnasDon/wacrm, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wacrm

## Pinned environment

- Project commit: `aee1b01f4b557870f1bbf9e7f566a2759e8f20f3`
- Test commit: `aee1b01f4b557870f1bbf9e7f566a2759e8f20f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 26.2 to 26.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 84 | 4.5 | 26.2 | 5 | 3 | [run](https://argusic.com/run/5626b65d-305f-4013-9887-ba6db8e1c725) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18.19.1 too old (project requires >=20, vitest 4 rolldown binding needs >=20.19)`
- 8 min: `npm install with Node 20 didn't install @rolldown/binding-linux-x64-gnu native binary`
- `Production next build OOM-killed (2 GB RAM, no swap)`
- `middleware.ts convention deprecated in Next.js 16 , should use proxy.ts instead`
- `Edge Runtime deprecated, middleware should use nodejs runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
