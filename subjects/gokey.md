# gokey

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudflare/gokey, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/gokey

## Pinned environment

- Project commit: `a5b5ea4b9bf968c7c5ece859287a31bdd1063a8d`
- Test commit: `a5b5ea4b9bf968c7c5ece859287a31bdd1063a8d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.3 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.25 | 3.3 | 0 | 0 | [run](https://argusic.com/run/a875f498-26e2-4ae1-933e-7860d3272a79) |
| 2 | pass | 100 | 2.1 | 5.8 | 2 | 2 | [run](https://argusic.com/run/cd968379-3171-4438-a361-131135b24a83) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Go not installed - downloaded go1.24.0.linux-amd64.tar.gz and extracted to /home/runner/go/go/`
- 0.2 min: `go vet: unkeyed fields in pkix.AlgorithmIdentifier struct literal at gokey.go:99 and :102`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
