# memento-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gannonh/memento-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/memento-mcp

## Pinned environment

- Project commit: `be6dc369784ecf8e6a7eced47b551f4b1f186e75`
- Test commit: `be6dc369784ecf8e6a7eced47b551f4b1f186e75`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 5.9 | 1 | 1 | [run](https://argusic.com/run/3fc12326-99e1-4e15-8d99-d3093f82afb3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Neo4j integration tests in Neo4jIntegration.test.ts tried to connect to a real Neo4j server that doesn't exist in this container, causing 3 test failures.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
