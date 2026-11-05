# infinite-canvas

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/basketikun/infinite-canvas, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/infinite-canvas

## Pinned environment

- Project commit: `dab19adc0847e32e39b7fc8ff90cb392561fb826`
- Test commit: `dab19adc0847e32e39b7fc8ff90cb392561fb826`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 22.1 to 32.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 32.2 | 4 | 4 | [run](https://argusic.com/run/06d4c5ba-e5f2-4cd5-ba85-8a60957e3069) |
| 2 | pass with mocks | 92 | 38 | 22.1 | 5 | 5 | [run](https://argusic.com/run/b73893de-e867-4b96-8a86-2690f5a59ee0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `@ant-design/pro-components@3.0.0-beta.3 requires antd@^5.11.2 but antd@^6.4.2 is specified in project`
- 1 min: `Node.js 18.19.1 too old for Vite 7 (requires >=20.19)`
- 1 min: `bun not found (required by test script)`
- 1 min: `vite build OOM after 8736 modules on 2GB RAM container`

Attempt 2:

- 6 min: `bun is not installed and system Node 18.19.1 is below Vite 7's Node 20.19+/22.12+ requirement`
- 3 min: `bun run dev crashed with TypeError: crypto.hash is not a function`
- 8 min: `bun run typecheck failed with TS2353 in model-script-editor.tsx: antd 6 Modal styles.content is not a valid property`
- 3 min: `Docs next build failed with Next.js requiring Node >=20.9.0 while bun run used system Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
