# fable51-worlds

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PhiloLabs/fable51-worlds, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/fable51-worlds

## Pinned environment

- Project commit: `d24028466530a15d58d3d94537e6317b84101589`
- Test commit: `d24028466530a15d58d3d94537e6317b84101589`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 64.1 to 64.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 64.1 | 3 | 3 | [run](https://argusic.com/run/de8b6108-8a20-4329-8d55-49ff6ea34614) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `death-star-trench-run package.json missing all runtime dependencies`
- 3 min: `union-square-sf vite 8 requires Node >=20 but container has Node 18`
- 2 min: `Playwright 1.62 requires Node >=20, incompatible with Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
