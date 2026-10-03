# caddy

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/caddyserver/caddy, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/caddy

## Pinned environment

- Project commit: `62a72977e58c87fad7e7726c18b58f10c653f2d3`
- Test commit: `62a72977e58c87fad7e7726c18b58f10c653f2d3`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 3.4 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 3.4 | 3 | 3 | [run](https://argusic.com/run/55426dbf-e406-486f-9036-4f276414fb6c) |
| 1 | pass | 100 | 2.5 | 5.2 | 0 | 0 | [run](https://argusic.com/run/0f759c53-53d3-4cfd-af58-695e7898ca29) |
| 2 | pass | 90 | 6 | 6.3 | 2 | 1 | [run](https://argusic.com/run/fc2f1286-8852-4973-b490-e2920e351609) |
| 3 | pass | 100 | 5 | 6.1 | 1 | 1 | [run](https://argusic.com/run/fee45826-7b6f-44de-bdac-c4b28ddede11) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.25 not installed in container`
- `/usr/local directory not writable`
- `No C compiler available; race detector requires CGO_ENABLED=1 with gcc`

Attempt 2:

- 2 min: `Go compiler not found in container`
- `certutil not available for system trust store (non-fatal)`

Attempt 3:

- 4 min: `Go 1.25.1 required but go binary not found in system`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
