# design.md

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google-labs-code/design.md, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/design-md

## Pinned environment

- Project commit: `9bf8eae67128b6cc55ad9bf86665767deb4c11cd`
- Test commit: `9bf8eae67128b6cc55ad9bf86665767deb4c11cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 3.4 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 9.6 | 1 | 1 | [run](https://argusic.com/run/b0f5bed0-13ea-46a4-8b72-b9922019d6ec) |
| 2 | pass | 100 | 16 | 3.8 | 1 | 1 | [run](https://argusic.com/run/73aec06a-4239-4658-9af3-641f8666c72d) |
| 3 | pass | 100 | 2 | 3.4 | 3 | 3 | [run](https://argusic.com/run/f69b1cf4-902d-4061-a09d-d17734f25163) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `bun not found in environment`

Attempt 2:

- 1 min: `bun executable not in PATH; tests spawning 'bun run' would fail`

Attempt 3:

- 0.5 min: `bun runtime not found (package manager expected by project)`
- `unzip not available in container`
- `turbo build fails: 'Unable to find package manager binary'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
