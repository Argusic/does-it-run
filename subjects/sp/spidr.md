# spidr

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/postmodern/spidr, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/spidr

## Pinned environment

- Project commit: `657b9db4f87a0db6616989b9a183c8327cfbaf80`
- Test commit: `657b9db4f87a0db6616989b9a183c8327cfbaf80`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 20.4 to 32.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 33 | 20.4 | 3 | 3 | [run](https://argusic.com/run/76974e41-cd7a-4cc1-9d6a-a3b0c58f63f2) |
| 2 | pass with mocks | 92 | 24 | 32.5 | 3 | 3 | [run](https://argusic.com/run/a01ee129-eb71-47b8-9c50-7ccf519ab6bf) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `No Ruby toolchain in container`
- 7 min: `Ruby stdlib extensions zlib, psych, fiddle could not build: no system dev headers for zlib, libyaml, libffi`
- 1 min: `Initial live check showed spider visited only /`

Attempt 2:

- 18 min: `Ruby not installed in container, built from source`
- 3 min: `zlib, psych, fiddle extensions not compiled during initial build (missing dev headers)`
- 1 min: `Sinatra 4.x HostAuthorization middleware blocks WebMock to_rack test apps`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
