# mianshiya

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/liyupi/mianshiya, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mianshiya

## Pinned environment

- Project commit: `7354f4859b7425338dfcff6410e9903bca0ec0dd`
- Test commit: `7354f4859b7425338dfcff6410e9903bca0ec0dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.9 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 12.9 | 5 | 5 | [run](https://argusic.com/run/01fc5b1e-7c9f-470e-83ae-2a6f70acdaf0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install failed with ERESOLVE peer dependency conflict (braft-editor requires react ^16 while project uses react ^17); yarn is not installed`
- 2 min: `umi/webpack build and dev failed under Node 18 with ERR_OSSL_EVP_UNSUPPORTED (webpack 5 MD4 hash rejected by OpenSSL 3)`
- 3 min: `Backend server crashed at startup with 'ReferenceError: File is not defined' from undici 7.30.1 (pulled transitively by cheerio 1.2.0, which requires Node 20 globals that Node 18.19 lacks)`
- 2 min: `Backend crashed on any request without an Origin header: ERR_HTTP_INVALID_HEADER_VALUE 'undefined' for Access-Control-Allow-Origin in server/src/server.js CORS middleware`
- `Database/auth-backed endpoints (question search, login, etc.) need real Tencent CloudBase env/secretId/secretKey plus Redis/MongoDB; the shipped config uses placeholder values (env 'mianshiya-xxx', secretId/secretKey 'xxx')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
