# page-agent

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alibaba/page-agent, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/page-agent

## Pinned environment

- Project commit: `9eb6b6646500264d9034dd466a4270cb9fc1ef1e`
- Test commit: `9eb6b6646500264d9034dd466a4270cb9fc1ef1e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4.6 to 26.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 26.9 | 2 | 2 | [run](https://argusic.com/run/699336e8-647e-42eb-93dc-1f940b2db67b) |
| 2 | pass with mocks | 92 | 6 | 4.6 | 1 | 1 | [run](https://argusic.com/run/d7217b2c-327a-4f94-a959-134883d8782f) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Built-in Node v18.19.1 does not satisfy engine requirement ^22.22.1 || >=24`
- 2 min: `npm run build:libs runs 5 Vite builds concurrently; unplugin-dts with TS6 OOM-kills core process under 2GB RAM and hangs 22+ min per package`

Attempt 2:

- 3 min: `npm install failed with Node v18.19.1 (required v22+). SyntaxError from wxt importing 'node:util'.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
