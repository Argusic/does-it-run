# youtube-automation-agent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/darkzOGx/youtube-automation-agent, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/youtube-automation-agent

## Pinned environment

- Project commit: `edbdbbd735169aeacb76cf28fe981b3009f214ea`
- Test commit: `edbdbbd735169aeacb76cf28fe981b3009f214ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.6 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 8.5 | 1 | 1 | [run](https://argusic.com/run/a5337e71-2574-4275-9be9-c0879463c25a) |
| 2 | pass | 100 | 2 | 5.6 | 1 | 1 | [run](https://argusic.com/run/df72e2f5-5cc6-464d-b90c-45996ef31743) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `testEngagementAIProviderWiring failed: OPENROUTER_API_KEY env var leaked into the test, causing AITextService to initialize from env vars instead of the credentials config object`

Attempt 2:

- 3 min: `Engagement AI Provider Wiring test failed because it only saved/restored OPENAI_API_KEY, but OPENROUTER_API_KEY was set in the container environment; the wrapped AITextService fell through to env vars`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
