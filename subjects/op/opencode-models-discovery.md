# opencode-models-discovery

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yuhp/opencode-models-discovery, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opencode-models-discovery

## Pinned environment

- Project commit: `f0fefdf96361a8d03c4e5d1b4fc5a731805ee945`
- Test commit: `f0fefdf96361a8d03c4e5d1b4fc5a731805ee945`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.9 to 16.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 16.9 | 6 | 6 | [run](https://argusic.com/run/fa1c3a28-001e-45c7-849e-1155415c5936) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `npm ci under default Node 18.19.1 skipped the Rolldown native binary, and Vitest 5 failed importing styleText from node:util`
- 7 min: `First public npm OpenCode preview host failed to load the plugin because ctx.provider.transform was unavailable`
- 3 min: `Host config was initially placed at XDG_CONFIG_HOME/opencode.json instead of the host-read XDG_CONFIG_HOME/opencode/opencode.json`
- 5 min: `Managed OpenCode service repeatedly failed to bind port 49374 and hung; debug config also hung`
- 3 min: `Mock provider returned non-streaming JSON for streamed chat completions, causing provider.invalid-output retries`
- 4 min: `CLI invocation with --model mock/alpha reported provider.no-route`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
