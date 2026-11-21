# apkstart

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RoutineMiku/apkstart, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/apkstart

## Pinned environment

- Project commit: `b8771d06b0aa6ba66980aaf7dcc6dfa950d284f0`
- Test commit: `b8771d06b0aa6ba66980aaf7dcc6dfa950d284f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2.3 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 2.3 | 3 | 3 | [run](https://argusic.com/run/fb8cd821-3b20-42e4-a7a8-41df84ed2355) |
| 2 | pass with mocks | 92 | 0.2 | 2.8 | 3 | 3 | [run](https://argusic.com/run/ac13c6f7-38b8-491d-b329-691ace049deb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `package.json restricts os to win32, blocking npm install on Linux`
- 3 min: `Node.js v18.19.1 installed but project requires >=20; nvm not available natively`
- 2 min: `@napi-rs/lzma-linux-x64-gnu native binding missing after npm install (optional dependency not fetched)`

Attempt 2:

- 0.3 min: `npm install blocked by package.json os constraint (win32) on Linux`
- 0.5 min: `test/auto-test.js: '重试矩阵' test failed - duplicate variants produced identical dedup keys`
- 0.1 min: `Node.js v18 installed but project requires >=20`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
