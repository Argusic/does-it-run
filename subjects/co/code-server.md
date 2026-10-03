# code-server

**Verdict: runs.** Argusic Score 70.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coder/code-server, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/code-server

## Pinned environment

- Project commit: `2b2f8b3d5c64e2f0bda876e4b1a95a79067ca01a`
- Test commit: `2b2f8b3d5c64e2f0bda876e4b1a95a79067ca01a`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run, no run possible
- Valid runs: 3; wall time 12.6 to 34.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 12.6 | 3 | 3 | [run](https://argusic.com/run/13680818-1d23-4754-8a94-7b62b9b22514) |
| 2 | pass | 100 | 30 | 34.4 | 7 | 7 | [run](https://argusic.com/run/54119361-0129-48a7-b05d-a87943a08ad0) |
| 3 | fail | 20 | n/a | 26.5 | 0 | 0 | [run](https://argusic.com/run/07180387-c684-4924-93dd-a3ba2f038546) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `git submodule init failed: commit 08d4889f not found in default fetch. VS Code ref needs manual --branch 1.135.0 clone`
- 5 min: `kerberos native module failed: missing libkrb5-dev (gssapi/gssapi.h)`
- 3 min: `Unit test app.test.ts failed: port 2 does not give EACCES in this containerized environment`

Attempt 2:

- 5 min: `Node.js v18 in container, project requires Node 24`
- 2 min: `Missing git submodule lib/vscode`
- 3 min: `kerberos native module build failed: missing gssapi/gssapi.h`
- 2 min: `kerberos build still failed: missing et/com_err.h`
- 8 min: `native-keymap build failed: missing X11/xkbfile headers and libraries`
- 1 min: `argon2 install script not approved by npm`
- `VS Code server (lib/vscode/out/server-main.js) not built`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
