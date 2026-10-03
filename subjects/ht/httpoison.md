# httpoison

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/edgurgel/httpoison, licensed MIT, written in Elixir.

Evidence and recordings: https://argusic.com/subject/httpoison

## Pinned environment

- Project commit: `18be3fe9c75de8f0de4e1d43d11cc98ff04f988c`
- Test commit: `18be3fe9c75de8f0de4e1d43d11cc98ff04f988c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.6 to 11.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 11.6 | 1 | 1 | [run](https://argusic.com/run/aa1000c0-e695-4087-959b-c7504147cd08) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `SSL test certificates in httparrot fixture (server.crt signed by server-ca.crt) had expired (notAfter=Sep 23 2026)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
