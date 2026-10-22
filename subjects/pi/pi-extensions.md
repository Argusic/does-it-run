# pi-extensions

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/narumiruna/pi-extensions, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-extensions

## Pinned environment

- Project commit: `aefbcc4702a2bfe2ade793d57f216773ab4f6b88`
- Test commit: `aefbcc4702a2bfe2ade793d57f216773ab4f6b88`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 50.2 to 50.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 50.2 | 4 | 4 | [run](https://argusic.com/run/641b7954-b205-4883-bd49-facbcebe2347) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npm install fails with 'Invalid comparator' for node-domexception override in npm 9.2`
- 2 min: `vitest 5.x requires Node >=22.12.0, but only Node 18 is in PATH`
- 1 min: `vitest 5.0.4 needs vite peer dependency - npm with --legacy-peer-deps didn't install it`
- 2 min: `Test 'snapshot backups expand a tilde-configured agent directory' fails: os.homedir() caches in forked vitest workers, so tilde expansion uses the real home even after HOME is changed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
