# cloudflare-os

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudflare/cloudflare-os, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cloudflare-os

## Pinned environment

- Project commit: `004ab773fad6d4fb7fe67be920a3ef37e46dc58a`
- Test commit: `004ab773fad6d4fb7fe67be920a3ef37e46dc58a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 32.9 to 32.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 32.9 | 4 | 4 | [run](https://argusic.com/run/f16df8c1-b349-456c-8ee1-770acffb42d1) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `System had Node v18.19.1, but pnpm 11.17.0 requires >=22.13`
- 0.5 min: `Node without --experimental-strip-types cannot run .ts files; vite-plus spawns subprocesses that don't inherit the flag`
- 3 min: `URLPattern is not a global in Node 23 (it's in node:url); 5 test files/ configs failed with 'URLPattern is not defined'`
- 0.5 min: `portal-boundaries test expected error text /native connector/ but code now produces a different message`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
