# voicy

**Verdict: runs with mocks.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/backmeupplz/voicy, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/voicy

## Pinned environment

- Project commit: `2b8960bbaa89d8141f0c46a67fff3f7f0748605d`
- Test commit: `2b8960bbaa89d8141f0c46a67fff3f7f0748605d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.3 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88 | 4 | 6.3 | 5 | 4 | [run](https://argusic.com/run/12228771-e359-4c62-a014-f4e20f1d5a70) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `yarn not installed and global npm install failed with EACCES (no write to /usr/local/lib/node_modules)`
- 3 min: `MongoDB absent from container (no mongod/docker) and no root to install it`
- 2 min: `scripts/local-whisper-worker-proof.js failed: spawn say ENOENT (script only supports macOS 'say' to synthesize sample audio)`
- 1 min: `test:worker-local-stt without VOICY_WHISPER_COMMAND/VOICY_WORKER_MODEL fails because no whisper binary ships with the repo`
- `qa:telegram-upload and test:telegram-runtime require a real Telegram bot token (or logged-in Chrome at CDP :9222, which is not installed), so they cannot run without real credentials`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
