# fastify-http-proxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fastify/fastify-http-proxy, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/fastify-http-proxy

## Pinned environment

- Project commit: `1ef4b3c66647f7bc3c93ac67c6946971308e0553`
- Test commit: `1ef4b3c66647f7bc3c93ac67c6946971308e0553`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.6 to 3.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.6 | 2 | 2 | [run](https://argusic.com/run/410ed392-a00f-4dd9-8595-fdad51984491) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm test's lint step crashed on system Node v18.19.1: ERR_REQUIRE_ESM requiring ESM find-up/index.js from neostandard (needs Node >=20)`
- 1 min: `examples/example.js calls reply.redirect(302, 'https://fastify.dev') with wrong argument order, so its /upstream/redirect route returns FST_ERR_BAD_STATUS_CODE 500; the origin produces the same 500 on its own`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
