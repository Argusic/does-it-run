# mcp

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BrowserMCP/mcp, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/2fb6d946-d7ff-42ec-b923-1aaa4ee8297d

## Pinned environment

- Project commit: `5f50da7c9fde7bd4a6cbc6f34696e7840037e824`
- Test commit: `5f50da7c9fde7bd4a6cbc6f34696e7840037e824`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.9 to 37 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.9 | 3 | 3 | [run](https://argusic.com/run/2fb6d946-d7ff-42ec-b923-1aaa4ee8297d) |
| 2 | pass | 93.33 | 58 | 37 | 3 | 2 | [run](https://argusic.com/run/58b91192-c610-4f13-b6d7-c52574c178c1) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18 installed (too old, needs 24+)`
- 2 min: `Chromium not found by Playwright test helpers`
- 1 min: `Chromium crashes with 'No usable sandbox!' in container`

Attempt 2:

- 12 min: `container lacked repo-required Node>=24 and pnpm 12.9.1 (had Node 18.19.1, no pnpm)`
- 10 min: `Chromium in tests and smoke died with 'No usable sandbox' (AppArmor blocks unprivileged user namespaces; CI uses a root-only sysctl)`
- 36 min: `pnpm smoke section 'another extension's iframe that comes back when removed' occasionally hits a frame-navigation race: 'The tab didn't become ready in time', cascading into the next 3 sections (14/18 on bad runs, 18/18 when benign)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
