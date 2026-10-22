# botonic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hubtype/botonic, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/botonic

## Pinned environment

- Project commit: `dcfdaa72d71b872d5f8a40a03097a2107292427b`
- Test commit: `dcfdaa72d71b872d5f8a40a03097a2107292427b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.6 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 10.6 | 3 | 3 | [run](https://argusic.com/run/218f74e9-8531-4ae9-8da1-35cad1bfdee9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Container Node was v18.19.1 but botonic engines/CI require Node >=22; worked around by downloading official Node v22.14.0 to /tmp/node22`
- 1 min: `Parallel package builds failed resolving '@botonic/core' because @botonic/core/lib was not built yet (build ordering race in my own command)`
- 2 min: `A bot created via 'botonic new myBot blank' failed 'npm test' with 'Cannot find module /tmp/myBot/babel.config.js' because the published @botonic/example-blank template (and examples/blank in-repo) lacks babel.config.js while its jest.confi`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
