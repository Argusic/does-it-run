# OpenCLI

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jackwener/OpenCLI, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/opencli

## Pinned environment

- Project commit: `8271afc67e8504bda94c147f446ee29775d08274`
- Test commit: `8271afc67e8504bda94c147f446ee29775d08274`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 16 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/54f48b3e-42bb-48e8-84b5-419934595c62) |
| 2 | pass | 100 | 15.8 | 16 | 4 | 4 | [run](https://argusic.com/run/ec1f556b-63df-43c3-baee-256435a1c272) |
| 3 | pass | 100 | 26 | 27.4 | 3 | 3 | [run](https://argusic.com/run/e9945e0f-4556-4a6e-bf1a-e07f713df514) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Node.js 18.19.1 in container , project requires >=20.18.1`
- 0.5 min: `Optional native dependency @rolldown/binding-linux-x64-gnu (1.2.5) not installed by npm ci due to npm optional-dependencies bug (npm/cli#4828)`
- 3 min: `CJS/ESM mismatch: html-encoding-sniffer (CJS) require()s @exodus/bytes/encoding-lite.js which is ESM-only , jsdom/29 downstream`
- `61 adapter test files fail , all require browser connections, third-party site access, or real credentials unavailable in this container`

Attempt 3:

- 1 min: `Node.js v18.19.1 too old, needs >=20.18.1`
- 1 min: `Missing rolldown native binding @rolldown/binding-linux-x64-gnu (npm optional dep bug)`
- 3 min: `@exodus/bytes ESM-only module incompatible with CJS require() in html-encoding-sniffer/jsdom caused infinite recursion under Node 20 --experimental-require-module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
