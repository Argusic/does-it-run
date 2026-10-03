# freshlytics

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sheshbabu/freshlytics, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/freshlytics

## Pinned environment

- Project commit: `75a167bafbc6af293ec02c107e1d704c30537e00`
- Test commit: `75a167bafbc6af293ec02c107e1d704c30537e00`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 13.6 to 33.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 34 | 33.9 | 7 | 7 | [run](https://argusic.com/run/97062dc5-c155-4af7-bf7e-bd93b1f8b946) |
| 2 | pass with mocks | 92 | 12 | 13.6 | 4 | 4 | [run](https://argusic.com/run/f5bc0107-594f-4350-9da5-7b9403a90420) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `bcrypt@3.0.6 native compilation fails on node 18 without C build tools`
- 1 min: `Webpack 4 ERR_OSSL_EVP_UNSUPPORTED on node 18`
- 4 min: `pg@7.11.0 protocol timeout with PostgreSQL 16`
- 2 min: `Seed script async calls unawaited; database not seeded`
- 8 min: `No PostgreSQL or Docker available in container`
- 5 min: `PipelineDB extension is proprietary/unavailable`
- 2 min: `DATABASE_URL with localhost resolves to IPv6 and fails`

Attempt 2:

- 1 min: `bcrypt@3.0.6 native module fails to compile on Node 18 (v8 API incompatibility)`
- 1 min: `webpack 4 fails on Node 18 with ERR_OSSL_EVP_UNSUPPORTED`
- 1 min: `Seed script had un-awaitend async call, admin user never created`
- 8 min: `No PostgreSQL or Docker available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
