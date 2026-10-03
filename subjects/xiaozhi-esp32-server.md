# xiaozhi-esp32-server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xinnan-tech/xiaozhi-esp32-server, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/xiaozhi-esp32-server

## Pinned environment

- Project commit: `788f5301fdd60cc3a8ef74025bfeece9b82b94ce`
- Test commit: `788f5301fdd60cc3a8ef74025bfeece9b82b94ce`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 7.2 | 3 | 3 | [run](https://argusic.com/run/c06bfd40-162f-42b8-b8ae-34ef20f06550) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `anyio pytest plugin conflicts with pytest-asyncio, causing AttributeError on async test collection`
- 1 min: `Empty data/.config.yaml causes NoneType error when loader calls .get() on yaml.safe_load result`
- `Java 21 and Maven not installed; manager-api Java component cannot build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
