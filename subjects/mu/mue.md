# mue

**Verdict: runs with mocks.** Argusic Score 84 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mue/mue, licensed BSD-3-Clause, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/mue

## Pinned environment

- Project commit: `678e1d71161303d89a9b7ed94ce39281b9bb0505`
- Test commit: `678e1d71161303d89a9b7ed94ce39281b9bb0505`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 3; wall time 3.7 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 4 | 3.7 | 0 | 0 | [run](https://argusic.com/run/114df059-f8ef-457e-aabb-6909567e025b) |
| 2 | fail | 80 | 5 | 4.5 | 2 | 2 | [run](https://argusic.com/run/62783a83-ad36-48d3-a09f-ebd278078175) |
| 2 | pass with mocks | 92 | 8 | 10.1 | 3 | 3 | [run](https://argusic.com/run/c22c98ea-81f3-4183-ac24-36a9e1b13801) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Bun not installed; Node v18 system too old for Vite 7 (requires >=20.19). 'bun install' fails without bun.`
- 1 min: `eslint-plugin-react@7.37.5 incompatible with ESLint 10: 'contextOrFilename.getFilename is not a function' during lint.`

Attempt 2:

- 2 min: `Node.js version in container is v18.19.1 but Vite requires >=20.19.0`
- 2 min: `Import 'SiTencentqq' does not exist in react-icons/si (react-icons v5.7.0)`
- 1 min: `ESLint 10 incompatible with eslint-plugin-react (getFilename API change)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
