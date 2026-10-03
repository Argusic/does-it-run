# chalk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chalk/chalk, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/chalk

## Pinned environment

- Project commit: `661317e6f91fe7c90306c2c48ea9354562ee9146`
- Test commit: `661317e6f91fe7c90306c2c48ea9354562ee9146`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 3.7 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.6 | 6 | 6 | [run](https://argusic.com/run/2bd66fe5-54c7-4536-87da-eb9502474bda) |
| 2 | pass | 100 | 6 | 8.5 | 3 | 3 | [run](https://argusic.com/run/75f22737-662e-44b9-8390-80b76560d912) |
| 3 | pass | 100 | 7 | 3.7 | 2 | 2 | [run](https://argusic.com/run/8d78b3e1-9508-402f-8d96-c34ce5d6013c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Ava v8 requires Node >=22 (uses 'with {type: 'json'}' import syntax)`
- 1 min: `Execa v10 requires Node >=20 (uses '/v' regex flag in internal code)`
- 1 min: `Test files instance.js, level.js, force-color.js used '/v' regex flag (Node >=20 feature)`
- `c8 coverage tool requires Node >=20 (uses ESM import in CJS context)`
- `xo linter requires Node >=22 (uses '/v' regex flag)`
- `typescript v6 requires Node >=22`

Attempt 2:

- 1 min: `System Node.js v18.19.1 does not meet chalk@6 requirement of Node >=22. The 'v' regex flag and 'with' type import assertions used by ava@8 and test files are unsupported in Node 18.`
- 1 min: `npm install with Node v18 produced engine warnings but did not install devDependencies. Subsequent install with Node v22 resolved this.`
- 1 min: `c8@12 requires ESM-only yargs, but Node v22.9.0 triggers ERR_REQUIRE_ESM from c8's CJS wrapper.`

Attempt 3:

- 3 min: `Node.js v18.19.1 is too old , chalk v6 requires >=22`
- `ava v8 requires Node >=22 for JSON module imports`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
