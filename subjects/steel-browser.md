# steel-browser

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/steel-dev/steel-browser, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/steel-browser

## Pinned environment

- Project commit: `2b41124d8e2953b0afe355c534e3c9aa71edae26`
- Test commit: `2b41124d8e2953b0afe355c534e3c9aa71edae26`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 10.1 to 17.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.1 | 3 | 3 | [run](https://argusic.com/run/ce100af9-0b1c-4752-bc51-fa96d9bfa5e6) |
| 2 | pass | 100 | 4 | 17.3 | 3 | 3 | [run](https://argusic.com/run/93a6c123-251d-48db-8bce-39c0ab3174e8) |
| 3 | pass | 100 | 9.1 | 11 | 5 | 5 | [run](https://argusic.com/run/212495e3-2f8b-481e-9840-112ded370f18) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 in container, project requires >=22`
- 4 min: `Chrome/Chromium not installed in container`
- 1 min: `Chrome binaries lacked executable permission (crashpad_handler)`

Attempt 2:

- 2 min: `Node.js v18.19.1 too old (package engines require >=22)`
- 1 min: `Chrome binary not found in container`
- `Chrome crash due to missing sandbox support (no root for suid sandbox, user namespace restrictions)`

Attempt 3:

- 1.5 min: `Container Node was v18 but repo requires >=22`
- 2 min: `No Chrome/Chromium binary present; puppeteer-core does not bundle one`
- 2 min: `Production-mode API crashed for non-root: FileService hardcodes mkdir '/files' (EACCES); Docker image runs as root so this is a container gap`
- 0.5 min: `Chrome launch failed: 'No usable sandbox' on Ubuntu 24.04 (non-root, user namespaces restricted)`
- 0.5 min: `Stale /tmp/steel-chrome SingletonLock from an earlier killed run blocked browser relaunch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
