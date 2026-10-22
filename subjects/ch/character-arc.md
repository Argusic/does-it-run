# character-arc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/uu201/character-arc, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/character-arc

## Pinned environment

- Project commit: `36b7be9d61a9ce5f70428b5e7e224d02c702e873`
- Test commit: `36b7be9d61a9ce5f70428b5e7e224d02c702e873`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.1 | 5 | 5 | [run](https://argusic.com/run/d6e6463a-a8f0-4c38-bca6-5756e57eeb68) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed on system; installed pnpm 10.33.2 to ~/.npm-global via npm install -g`
- 1 min: `Electron 37 SUID chrome-sandbox not configured (no root): 'The SUID sandbox helper binary was found, but is not configured correctly'`
- 2 min: `pnpm run build failed with 'crypto.hash is not a function' in @vitejs/plugin-vue because system Node is 18.19.1 (Vite 7 requires Node >=20.19)`
- 1 min: `npm script 'test' uses Windows-only 'set ELECTRON_RUN_AS_NODE=1&&' syntax, unusable on Linux/macOS shell`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
