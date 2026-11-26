# pinescript-ai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/arturoabreuhd/pinescript-ai, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pinescript-ai

## Pinned environment

- Project commit: `deb19882100a63af4afb6e174c0df72c14ce0053`
- Test commit: `deb19882100a63af4afb6e174c0df72c14ce0053`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 3.9 | 3 | 3 | [run](https://argusic.com/run/d3363f68-0117-4f1f-baf4-2160d37d3dd1) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18.19.1 too old for Next.js 16 (needs >=20.9.0)`
- 2 min: `Missing @tailwindcss/oxide-linux-x64-gnu native binding (npm optional dependency bug)`
- 1 min: `Optional dependency @opusaether/pine-transpiler not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
