# ethora

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dappros/ethora, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ethora

## Pinned environment

- Project commit: `0f289ba4b045c309bfff3afc2f602faafbed7e33`
- Test commit: `0f289ba4b045c309bfff3afc2f602faafbed7e33`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 6.2 to 78 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 77 | 78 | 8 | 8 | [run](https://argusic.com/run/cbf84fca-fb7d-4a9f-855a-3b683af87791) |
| 2 | pass | 100 | 2.5 | 6.2 | 2 | 2 | [run](https://argusic.com/run/81d4633b-3aa1-4e29-9bce-eebf3c25738a) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `sdk-reactjs: npm install fails (exit 137, OOM) because the package.json 'prepare' script runs two full tsc+vite builds; container has 2GB RAM, no swap`
- 6 min: `sdk-reactjs build fails: Vite 7.3.1 (pinned by package.json) requires Node >=20.19, container had Node 18.19.1 and no nvm; system root unavailable`
- 30 min: `sdk-reactjs production build still OOM-killed by the container during vite bundle phase (peak ~1.45GB RSS vs 2GB total incl. agent) even at max-old-space-size=1500`
- 12 min: `api/tags.js was invalid JavaScript (missing commas between exported tag objects), causing api/index.js (Swagger middleware) to throw SyntaxError and the api/ docs component to be unusable`
- 18 min: `setup CLI verification: initial scripted drive accidentally used the real Cloud QA API (network reachable) instead of my mock, writing a real profile`
- 6 min: `sdk-reactnative: hooksBundle.test.tsx 'usePendingNotification' test fails deterministically (asserts AsyncStorage cleared before the asynchronous effect completes); repo test at __tests__/hooksBundle.test.tsx:335`
- 5 min: `sdk-android / sdk-swift / sample-android / sample-swift: no JDK/Gradle/Swift toolchain in container (java, swifc, xcodebuild all absent), and sdk-wordpress needs a PHP interpreter (php absent) - cannot install without root`
- 3 min: `mcp-cli --http ignores ETHORA_MCP_PORT env and always listens on :3030`

Attempt 2:

- `Pre-existing test failure in sdk-reactnative hooksBundle.test.tsx:335 - AsyncStorage assertion (usePendingNotification test reads pending jid before it's cleared)`
- `npm WARN EBADENGINE eventsource-parser@3.0.3 requires node >=20.0.0, current is v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
