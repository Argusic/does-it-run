# openwiki

**Verdict: runs.** Argusic Score 92.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/langchain-ai/openwiki, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/6d4b3313-892e-449e-9a27-916695c492d2

## Pinned environment

- Project commit: `60c8eea57004e064eda4ae8395f6fde8172a8aec`
- Test commit: `60c8eea57004e064eda4ae8395f6fde8172a8aec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.2 to 10.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 3.2 | 0 | 0 | [run](https://argusic.com/run/6d4b3313-892e-449e-9a27-916695c492d2) |
| 2 | pass with mocks | 85.33 | 8 | 10.9 | 6 | 4 | [run](https://argusic.com/run/5839c5ea-a411-4983-a928-d91113c1c24a) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Container Node.js v18.19.1 is below the required >=22.22.0 and pnpm is absent`
- 1 min: `Corepack enable failed because the requested install directory did not exist`
- 8 min: `Visualizer printed stopped. and closed its port after SIGINT but the Node process remained alive`
- 1 min: `Documented --version is unsupported and exits 1 with Unknown option: --version`
- 2 min: `Installed openwiki 0.7.3 crashes with an Ink raw-mode error when --help output is piped`
- 3 min: `The first mock page submission was rejected because factual pages require at least one evidence-backed Claim`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
