# codex-plusplus

**Verdict: could not verify.** Argusic Score 13.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/b-nnett/codex-plusplus, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/codex-plusplus

## Pinned environment

- Project commit: `bf81723554bebc9a51e239dbca9c7b7247c628b5`
- Test commit: `bf81723554bebc9a51e239dbca9c7b7247c628b5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.9 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 13.33 | 45 | 2.9 | 3 | 2 | [run](https://argusic.com/run/ca4b31b0-3c63-449f-a7ed-4ef61aac0327) |
| 2 | fail | 13.33 | 18 | 4.4 | 3 | 2 | [run](https://argusic.com/run/0c1c259b-bb95-4836-aa18-50c262fbb18f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node v18.19.1 test crash: Object.groupBy is not a function in Tests/native-trace.test.mjs`
- 4 min: `Node v18.19.1 test crash: crypto is not defined in Tests/sidebar-adapter.test.mjs`
- 30 min: `Project declares macOS-only Swift package (platforms .macOS(.v14), AppKit/Security imports) and container is Ubuntu with no swift toolchain and no root`

Attempt 2:

- 13 min: `Swift/macOS build cannot run in this Linux container: no swift toolchain, Xcode, clang, or Apple frameworks (AppKit/WebKit/JavaScriptCore/Security/ServiceManagement); scripts/build-app.sh and swift test are macOS-only.`
- 2 min: `Tests/native-trace.test.mjs: Object.groupBy is not a function (Node 18 lacks Node 21+ API).`
- 3 min: `Tests/sidebar-adapter.test.mjs: 'crypto is not defined' in vm sandbox; Node 18 ESM has no global crypto and the parser context had none.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
