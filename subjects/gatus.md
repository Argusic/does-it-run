# gatus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/TwiN/gatus, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/gatus

## Pinned environment

- Project commit: `4d15cb7eed6225ac0b03da3d2ab50c424b81c34c`
- Test commit: `4d15cb7eed6225ac0b03da3d2ab50c424b81c34c`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 5.7 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 11.3 | 2 | 2 | [run](https://argusic.com/run/62546d4e-8c01-44eb-8721-ce4c700ba41e) |
| 2 | pass | 100 | 4.2 | 5.7 | 4 | 4 | [run](https://argusic.com/run/213c12ce-28b5-4739-a10d-32a918a63cfc) |
| 3 | pass | 100 | 45 | 6.5 | 3 | 3 | [run](https://argusic.com/run/20f0f666-d028-452e-804e-496f953c8cf8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `TestPing: ICMP ping to 127.0.0.1 requires CAP_NET_RAW capability for raw sockets, not available in container`
- 1 min: `TestIntegrationEvaluateHealthForICMP: ICMP health check to icmp://127.0.0.1 fails for same CAP_NET_RAW reason`

Attempt 2:

- 1.5 min: `Go 1.26.3 not found in PATH`
- 0.5 min: `Default config path config/config.yaml does not exist; config.yaml is at repo root`
- `TestPing fails: needs raw socket capabilities`
- `TestQueryDNS fails: DNS query to 8.8.8.8 times out`

Attempt 3:

- 7 min: `Go not installed in container , missing /usr/local/go`
- `TestPing fails , ICMP needs CAP_NET_RAW`
- `TestIntegrationEvaluateHealthForICMP fails , same ICMP privilege issue`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
