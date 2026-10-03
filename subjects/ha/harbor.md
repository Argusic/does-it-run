# harbor

**Verdict: runs with mocks.** Argusic Score 66 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/av/harbor, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/harbor

## Pinned environment

- Project commit: `4c20a822f61e912ebf8c57a362315f09c5080230`
- Test commit: `4c20a822f61e912ebf8c57a362315f09c5080230`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 8.2 to 16.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass with mocks | 82 | 12 | 16.5 | 4 | 2 | [run](https://argusic.com/run/79ab4810-9469-4cb1-99b3-4815fbcb51e8) |
| 2 | fail | 50 | 10 | 8.2 | 1 | 1 | [run](https://argusic.com/run/d4f88a2d-73bb-4bdd-b578-62c156beb0e8) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Deno lockfile version mismatch (v5 from newer Deno, installed Deno 2.2.0 writes v4)`
- 2 min: `Deno not installed in container`
- `Docker daemon not available (no root access)`
- `shellcheck not installed (optional, used by lint)`

Attempt 2:

- 15 min: `Docker daemon not available , running inside a restricted container without Docker socket, root access, rootless prerequisites (SUID newuidmap, slirp4netns), or cgroupv2 write permissions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
