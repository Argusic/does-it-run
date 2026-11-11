# Restfox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/flawiddsouza/Restfox, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/restfox

## Pinned environment

- Project commit: `74ba395f84993297146e70805e2cc1c6a03f21c7`
- Test commit: `74ba395f84993297146e70805e2cc1c6a03f21c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4 | 3 | 3 | [run](https://argusic.com/run/000af871-c1cf-4254-9e38-8e5e92412f63) |
| 2 | pass | 100 | 9 | 9.1 | 2 | 2 | [run](https://argusic.com/run/3016f312-2ecd-4f8b-8989-972e72c8fcfd) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `vite build: fatal: No names found, cannot describe anything`
- 1.5 min: `ReferenceError: File is not defined in undici with Node 18.19.1`
- 1 min: `TypeError: Cannot read properties of undefined in undici decompress with Node 22.14.0`

Attempt 2:

- 6 min: `Node.js v18.19.1 is installed by default, but the project requires Node >=26 for web-standalone and undici 8 compat. tls.getCACertificates/setDefaultCACertificates APIs are missing, undici 8 fails to load, and SOCKS5 proxy tests fail.`
- 1 min: `vitest config did not exclude node_modules_backup directory, causing test pollution from old electron-log and other specs.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
