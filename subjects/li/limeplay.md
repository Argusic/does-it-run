# limeplay

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WINOFFRG/limeplay, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/limeplay

## Pinned environment

- Project commit: `eef715868500c30b589c7fcddea6ca667c10c838`
- Test commit: `eef715868500c30b589c7fcddea6ca667c10c838`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.5 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.27 | 8.5 | 3 | 3 | [run](https://argusic.com/run/c0e9a92e-becc-4938-9051-e195a2088e9b) |

## What was observed on a clean machine

Attempt 1:

- 0.27 min: `Container has Node 18 (project requires 23+) and no Bun (project requires bun 1.2.19)`
- 0.1 min: `Registry build: shadcn child process used system Node 18, which lacks global File() type needed by undici v7`
- 0.02 min: `Registry install integration test: script calls 'bunx' but zip-only Bun install had no bunx shim`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
