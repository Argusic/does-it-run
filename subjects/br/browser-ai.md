# browser-ai

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jakobhoeg/browser-ai, licensed NOASSERTION, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/browser-ai

## Pinned environment

- Project commit: `a53509d4f923cf85340fa7eef17ba8ac189d3892`
- Test commit: `a53509d4f923cf85340fa7eef17ba8ac189d3892`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 4; wall time 5.4 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 23.9 | 2 | 2 | [run](https://argusic.com/run/19e8eed1-4f3d-4313-8915-cdbc30616f91) |
| 1 | pass | 100 | 2 | 5.4 | 2 | 2 | [run](https://argusic.com/run/3d6b2b6b-7759-4b1c-a83e-155719e266e6) |
| 2 | pass | 100 | 18 | 23 | 3 | 3 | [run](https://argusic.com/run/aeefd7d1-449c-43e7-93ca-fe87228718fc) |
| 3 | pass with mocks | 92 | 1.75 | 22.7 | 5 | 5 | [run](https://argusic.com/run/326d0936-1e42-4ccd-bdfc-d7f50e0d4a88) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Vitest 4.x requires Node >=20 but container has Node 18.19.1`
- 1 min: `docs (Next.js 16) requires Node >=20.9.0 but container has Node 18.19.1`

Attempt 1:

- 2 min: `Node.js v18.19.1 is incompatible with vitest v4.1.0 and vite v7.x , vitest v4 uses ESM-only std-env which cannot be require()'d in Node 18`
- `docs package (Next.js docs site) requires Node >=20.9.0, fails to build under Node 18`

Attempt 2:

- 8 min: `vitest@4.x requires Node >= 20 (container has 18.19)`
- 3 min: `jsdom@28.x requires Node >= 20`
- 2 min: `vite@6.x requires Node >= 20`

Attempt 3:

- 6.5 min: `Vitest 4.1.0 requires Node >=20 but container has Node 18.19.1 - ERR_REQUIRE_ESM on std-env ESM module from CJS vitest config`
- 2.1 min: `jsdom 28.1.0 requires Node >=22 (html-encoding-sniffer -> @exodus/bytes ESM-only), causing ERR_REQUIRE_ESM`
- 1 min: `transformers-js transcription test fails with 'window is not defined' because Node environment lacks window/AudioContext globals`
- 0.7 min: `transformers-js DTS build fails: 'return_tensors' does not exist in type (should be 'return_tensor')`
- 0.3 min: `Docs/Next.js build fails because Node 18 is below >=20.9.0 requirement`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
