# pomerium

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pomerium/pomerium, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/pomerium

## Pinned environment

- Project commit: `35d2936ae76795cf8edc44d25f0c49b7cbce8265`
- Test commit: `35d2936ae76795cf8edc44d25f0c49b7cbce8265`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.5 to 82.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 82.9 | 3 | 3 | [run](https://argusic.com/run/697af496-7a55-439e-a082-2e73b9b5706c) |
| 2 | pass | 92 | 8 | 9.5 | 5 | 3 | [run](https://argusic.com/run/44c58726-ce0b-453d-821a-32c3c9692260) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.1 not installed in container`
- 2 min: `Envoy binary not embedded in pkg/envoy/files/`
- 1 min: `Lockfile checksum mismatch from initial zero-byte stub`

Attempt 2:

- 1 min: `go: not found in PATH`
- 1 min: `go build failed: embedded envoy-linux-amd64 binary missing`
- 1 min: `backgrounded pomerium server was killed when its launching shell exited`
- 1 min: `pkg/storage/postgres and pkg/storage/blob tests need Docker testcontainers (Postgres/SeaweedFS)`
- 1 min: `config/envoyconfig TestBuildListeners/quic fails: expected UDP address '::' vs actual '0.0.0.0'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
