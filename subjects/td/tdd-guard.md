# tdd-guard

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nizos/tdd-guard, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tdd-guard

## Pinned environment

- Project commit: `ccd71b49b11b5bd350d87d3f4c9a9b6b1e1f3dbd`
- Test commit: `ccd71b49b11b5bd350d87d3f4c9a9b6b1e1f3dbd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 26.9 to 52.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 26 | 26.9 | 9 | 9 | [run](https://argusic.com/run/1a1bdc66-0b73-4203-845a-831741a3da49) |
| 2 | pass with mocks | 92 | 3 | 52.8 | 5 | 5 | [run](https://argusic.com/run/f852c1b1-07d4-4a4d-8282-1fe0bd2ba8f7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js >=22 required, only 18 available`
- 3 min: `Golangci-lint tests fail: buildArgs uses deprecated --output.json.path=stdout and --path-mode=abs flags not supported in golangci-lint v1.60.2`
- 2 min: `Python/pytest reporter unavailable , no venv with pytest installed`
- 1 min: `Go reporter not built`
- 2 min: `Rust reporter not built`
- 1 min: `RuboCop linter tests fail , Ruby not available`
- 1 min: `PHP, Storybook, JUnit5, RSpec, Minitest reporters unavailable , missing language runtimes (PHP, Ruby, Node/Playwright)`
- 1 min: `1 AI model test fails (validationResponse.test.ts) , need real credentials`

Attempt 2:

- 2 min: `Node.js 18 system install; project requires Node.js 22+`
- 2 min: `golangci-lint tests failed: Go not installed`
- 8 min: `RuboCop tests failed: Ruby not installed; rubocop gem missing libyaml dependency`
- 10 min: `Reporter integration tests: PHP, Rust, Storybook, RSpec, Minitest, JUnit5 reporters need missing language runtimes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
