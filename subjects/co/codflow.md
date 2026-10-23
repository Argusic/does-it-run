# codflow

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bighadj22/codflow, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codflow

## Pinned environment

- Project commit: `025bc9cb000a378d1002e385eb01b20164a0748d`
- Test commit: `025bc9cb000a378d1002e385eb01b20164a0748d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.3 to 17.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 17.3 | 4 | 4 | [run](https://argusic.com/run/b0298ab1-0291-4dcf-9270-dab44e156cb8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 pre-installed but project requires >=22.12.0`
- 3 min: `Initial npm ci installed native bindings under Node 18, causing rolldown/vitest startup failure ('Cannot find native binding')`
- `wrangler dev fails locally , @cloudflare/workers-oauth-provider requires HTTPS in authorization_servers; http://localhost is rejected. This blocks every route including / and /health`
- 1 min: `wrangler dev also hit EMFILE (too many open files) on first attempt due to default ulimit; re-ran with fresh terminal`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
