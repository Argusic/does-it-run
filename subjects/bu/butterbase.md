# butterbase

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/butterbase-ai/butterbase, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/butterbase

## Pinned environment

- Project commit: `b8623ece2ad7756a89578434102c3f40926c653e`
- Test commit: `b8623ece2ad7756a89578434102c3f40926c653e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 14.2 to 38.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 14.2 | 0 | 0 | [run](https://argusic.com/run/6be275dd-0d27-4766-b2ed-536dde598f87) |
| 2 | pass with mocks | 92 | 36 | 38.2 | 4 | 4 | [run](https://argusic.com/run/ed6a32ff-8f70-491c-8493-1212e093cfda) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `npm install fails with 'Cannot set properties of null (setting peer)' - npm 9.2.0 too old for this workspace`
- 2 min: `pnpm blocks build scripts for argon2, bcrypt, esbuild, sharp, workerd`
- 2 min: `crypto.randomUUID undefined in Node v18, breaking quota-enforcer test`
- `280 control-api tests fail due to missing Postgres/Redis (no Docker available)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
