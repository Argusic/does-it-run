# gstack

**Verdict: runs.** Argusic Score 97.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/garrytan/gstack, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/gstack

## Pinned environment

- Project commit: `07b59e396c6be5a86619a43151cb9ed62a15ae69`
- Test commit: `07b59e396c6be5a86619a43151cb9ed62a15ae69`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 5; wall time 12.5 to 65.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.5 | 1 | 1 | [run](https://argusic.com/run/a6b9f690-b667-4406-bcb9-cf82462075ce) |
| 1 | pass with mocks | 92 | 42 | 27.3 | 3 | 3 | [run](https://argusic.com/run/0efd4cf1-79fb-4ed9-b6b8-8de2c14cec73) |
| 1 | pass | 96.67 | 8 | 22.2 | 6 | 5 | [run](https://argusic.com/run/23e03703-edbf-4152-8d57-94fb10afb15a) |
| 2 | pass | 100 | 15 | 15.4 | 5 | 5 | [run](https://argusic.com/run/2f7710e6-96d6-48e7-9f44-2f1f35b41942) |
| 3 | pass | 100 | 5 | 65.1 | 6 | 6 | [run](https://argusic.com/run/10b967a6-f0b2-48d1-8a09-a2ed21964dce) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Bun not installed in container`

Attempt 1:

- 5 min: `Playwright Chromium browser binaries not installed - container lacks browser environment`
- `Git commit failures in test environment - cannot write to repo`
- 8 min: `System Node.js v18 too old for Playwright v1.62.1`

Attempt 1:

- 1 min: `bun not found in container`
- 1 min: `Playwright requires Node.js >= 20, system has Node 18`
- `Chromium sandbox fails in container (no CONTAINER env var set)`
- `'file --mime-type' command not available for binary detection test`
- `git user.name and user.email not configured`
- `Bun.spawnSync(['node', ...]) finds system Node 18 instead of nvm Node 22`

Attempt 2:

- 2 min: `Bun not found in system PATH`
- 1 min: `Node.js 18 too old for Playwright (needs 20+)`
- 2 min: `Chromium sandbox fails in container (unprivileged user namespaces disabled)`
- 2 min: `bun .exe suffix prevents PATH resolution (npm package ships bun.exe, not bun)`
- 2 min: `file command not found, causing test/skill-validation.test.ts to fail on Mach-O/ELF binary detection`

Attempt 3:

- 1 min: `Bun binary not on PATH (stored as 'bun.exe' in npx cache)`
- 2 min: `Playwright Chromium not installed , Node.js 18.19.1 blocks 'npx playwright install'`
- 1 min: `'file' command missing from container image`
- 1 min: `Chromium sandbox fails in container (unprivileged user namespaces disabled)`
- `Git config not set globally; session-update tests failed`
- 5 min: `3/6 test shards passed fully (4444 tests); 3 remaining shards fail from browser sandbox/timing/env-propagation to subprocess shards (not code defects)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
