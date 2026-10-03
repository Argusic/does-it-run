# n8n-skills

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/czlonkowski/n8n-skills, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/n8n-skills

## Pinned environment

- Project commit: `19cd793f4789e3ef9c657ccf26e097f641a77df0`
- Test commit: `19cd793f4789e3ef9c657ccf26e097f641a77df0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 6.1 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 5 | 6.1 | 1 | 1 | [run](https://argusic.com/run/ebf74e51-2f2d-4e5c-a78e-d04f8565586c) |
| 2 | pass with mocks | 92 | 4.5 | 8.3 | 4 | 4 | [run](https://argusic.com/run/a4c7069c-61ee-44e2-9b4e-2c2107f33690) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `build.sh failed at line 68: 'zip' command not found (no root to install it)`

Attempt 2:

- 0.5 min: `zip: command not found`
- 0.5 min: `npm install -g n8n-mcp: EACCES on /usr/local`
- `Node v18.19.1 < required >=20.0.0, engine warnings`
- 0.5 min: `mcp.json points to remote HTTPS endpoint (401 unauthorized)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
