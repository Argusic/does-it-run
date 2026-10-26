# open-vetta

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openvetta/open-vetta, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-vetta

## Pinned environment

- Project commit: `fa6c1df3a28d3a1d8c6906589aa6d01f7e192f90`
- Test commit: `fa6c1df3a28d3a1d8c6906589aa6d01f7e192f90`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 15 | 5 | 5 | [run](https://argusic.com/run/9d510f0d-9bc9-46f0-88bf-eecc65e1284a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Bun runtime not pre-installed; Node.js 18.x instead of required 20+`
- `theme-ui: 2 E2E markdown-link tests fail due to require() of ESM unified module from CJS react-markdown`
- `Desktop tsc type-checking runs out of memory (773MB limit, ~2GB needed)`
- `Docs-site build fails: Next.js Turbopack loader fails on fumadocs-mdx ESM/CJS boundary`
- `Vite requires Node 22.12+ (we have 22.11.0) but builds still succeed for all 14 presets`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
