# APIAuto

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TommyLemon/APIAuto, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/apiauto

## Pinned environment

- Project commit: `f2042ae79d1420d341bfc831d7c9bfb347ad2c7e`
- Test commit: `f2042ae79d1420d341bfc831d7c9bfb347ad2c7e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 2.8 | 1 | 1 | [run](https://argusic.com/run/133fa3c3-54aa-4bc2-8400-9201fcbbe369) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `SyntaxError: Cannot use import statement outside a module in js/main.js:87-88 , two import statements with ES module syntax inside a require()-based eval() block in the Node.js path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
