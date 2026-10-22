# spring-ai-agent-utils

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spring-ai-community/spring-ai-agent-utils, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/spring-ai-agent-utils

## Pinned environment

- Project commit: `fe1255dc5640c78d810169898ed500da2410cb3b`
- Test commit: `fe1255dc5640c78d810169898ed500da2410cb3b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 0.5 | 8 | 1 | 1 | [run](https://argusic.com/run/08b71853-a779-4ff0-a1a7-f9f6a79dc9ce) |
| 2 | pass | 100 | 5 | 9.7 | 3 | 3 | [run](https://argusic.com/run/86fe7b8a-e6d7-4732-8794-bf749339e743) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Example apps require real third-party AI API keys (ANTHROPIC_API_KEY, OPENAI_API_KEY, or GOOGLE_CLOUD_PROJECT with GCP service account credentials) at startup - Google GenAI SDK validates credentials before any API call`

Attempt 2:

- 2 min: `Neither Java nor Maven were installed in the container`
- 1 min: `Initial Maven 3.9.9 download returned 404, required fallback to 3.9.8`
- `3 tests were skipped (ShellToolsTest CrossPlatformCompatibility and GrepToolTest GlobAndTypeFilter) , expected platform-specific skips`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
