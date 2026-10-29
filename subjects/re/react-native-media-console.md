# react-native-media-console

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LunatiqueCoder/react-native-media-console, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/react-native-media-console

## Pinned environment

- Project commit: `0ae7dc4d23a5687090b67693b76b061b4ecefcae`
- Test commit: `0ae7dc4d23a5687090b67693b76b061b4ecefcae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.8 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 17.8 | 5 | 5 | [run](https://argusic.com/run/d5e0e3ff-238e-4e03-8152-657928f39152) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No yarn or corepack bundled; global npm install of yarn failed with EACCES on /usr/local/lib/node_modules`
- 2 min: `yarn install succeeded but jest-expo could not parse react-native Flow files: MyTVProject had no babel.config.js`
- 3 min: `expo export (web and android) was OOM-killed (exit 137, 'Killed') with default workers`
- 2 min: `Repo turbo pipeline is broken: turbo run build fails 'Could not find react-native-media-console#prepare' and turbo run prepare fails 'could not find task prepare in project'`
- `Root yarn tsc -p tsconfig.json reports @/ alias resolution errors in examples/MyTVProject (Cannot find module '@/hooks/...' etc.) and React UMD-global errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
