# youtube-music

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sohaibdevv/youtube-music, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/youtube-music

## Pinned environment

- Project commit: `1a7c97858595ac7db173a18a83d66f46c653a41d`
- Test commit: `1a7c97858595ac7db173a18a83d66f46c653a41d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.8 | 3 | 3 | [run](https://argusic.com/run/0d16f3b1-d13b-462c-a185-0525c25d5569) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found on PATH`
- 1 min: `ERR_PNPM_UNSUPPORTED_ENGINE: node 22.12.0 did not satisfy node-gyp requirement ^22.22.2`
- 0.5 min: `Cannot find module dist/main/index.js -- electron test requires built app`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
