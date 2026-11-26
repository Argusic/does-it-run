# mern-marketplace

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shamahoque/mern-marketplace, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/mern-marketplace

## Pinned environment

- Project commit: `bf3fc45e7782b13dcaefdae8939c621a3c9a65e3`
- Test commit: `bf3fc45e7782b13dcaefdae8939c621a3c9a65e3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 6.2 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 6.2 | 2 | 2 | [run](https://argusic.com/run/75291c95-f6a3-4648-b8ab-df109c7abbf5) |
| 2 | pass with mocks | 92 | 18 | 7.4 | 4 | 4 | [run](https://argusic.com/run/e3b34f52-2713-4711-a7ac-93ca96d3570c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `webpack 4 build crashes on Node 18/OpenSSL 3 with ERR_OSSL_EVP_UNSUPPORTED (MD4 hash unsupported)`
- 4 min: `MongoDB 4.2.24 prebuilt binary fails to load: libcrypto.so.1.1 not found on Ubuntu 24.04 (OpenSSL 3 only)`

Attempt 2:

- `Node version mismatch (require 13.12.0, have 18.19.1)`
- 2 min: `MongoDB not installed in container`
- 1 min: `ERR_OSSL_EVP_UNSUPPORTED from OpenSSL 3 / Node 18 during webpack build`
- `yarn not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
