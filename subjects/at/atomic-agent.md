# atomic-agent

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AtomicBot-ai/atomic-agent, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/atomic-agent

## Pinned environment

- Project commit: `f31ec05d91254e10a5a05598d711f33f8cf85d42`
- Test commit: `f31ec05d91254e10a5a05598d711f33f8cf85d42`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 25.6 to 58.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 58.1 | 2 | 2 | [run](https://argusic.com/run/7e63a2a3-05f4-49ad-a765-0942c753eca8) |
| 2 | pass with mocks | 92 | 5 | 25.6 | 3 | 3 | [run](https://argusic.com/run/66f37cc3-e3d2-4952-9538-20f6dbeb3c33) |

## What was observed on a clean machine

Attempt 1:

- `src/sidecar/send-message-concurrency.test.ts: expects 2 LLM entries but runtime produces 5 (extra work from background reflection/memory calls)`
- `3 tests timeout (30000ms) due to resource contention when running full parallel suite: fusion-delegate.integration.test.ts, abortable-subcall.network.test.ts, sidecar/local-probe-gating.test.ts`

Attempt 2:

- 2 min: `Container had Node.js v18.19.1 but project requires >=25.7.0 , npm install emitted EBADENGINE warnings and strict-pinned deps like better-sqlite3 would fail at build`
- 10 min: `Test 'sidecar send_message concurrency > serialises two rapid send_message calls FIFO without crossing state' failed , llamaComplete mock only guarded 'reflection:' prefix but memory-v2 features (rewriter, link-gen, vote, distill, title) ar`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
