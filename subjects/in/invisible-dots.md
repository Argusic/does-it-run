# invisible_dots

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/feder-cr/invisible_dots, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/invisible-dots

## Pinned environment

- Project commit: `5afd5f066ee708b2438652d706028b2716d993c8`
- Test commit: `5afd5f066ee708b2438652d706028b2716d993c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 21.8 to 48.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 48.6 | 1 | 1 | [run](https://argusic.com/run/219d5513-db53-4f1c-8d92-5a3bdbdc7d38) |
| 2 | pass | 96 | 22 | 21.8 | 5 | 4 | [run](https://argusic.com/run/2156d4a8-a9ae-4cb0-8414-ce58268bb699) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Node.js v18.19.1 too old (project requires Node 24+); readline in Node 24.21 treats \u007f (DEL) literally on in-memory streams instead of as backspace`

Attempt 2:

- 6 min: `@asamuzakjp/css-color@7.1.3 requires node ^22.22.2 || ^24.15.0 || >=26.0.0; container had Node 18, and Node 24.11.1 was too old for npm ci (EBADENGINE)`
- 20 min: `vitest failed 1 test: apps/cli/test/secret-input.test.ts expected '123456:AABBCC' but got '123456:AABBxx\u007f\u007fCC'`
- 12 min: `go test failed TestExecEnvIsTheAccountsNotTheDaemons: DISPLAY = ":99", want ":0" (inherited Xvfb DISPLAY leaked into execEnv)`
- 8 min: `invisible-dots server exited with EADDRINUSE on 127.0.0.1:8787 because the harness's argusic proxy already holds that port`
- 3 min: `A created Dot went to ERROR: 'cannot list the images directory /tmp/idots-home/images: ENOENT' because there is no QEMU, no /dev/kvm and no root to install them`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
