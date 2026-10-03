# jaeger

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jaegertracing/jaeger, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/jaeger

## Pinned environment

- Project commit: `473822d2189c4d173da44aeda17261cfc05ad82f`
- Test commit: `473822d2189c4d173da44aeda17261cfc05ad82f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.1 to 23.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 23.1 | 2 | 2 | [run](https://argusic.com/run/cf851a84-1dc1-4b10-8f0a-d4643c2873e2) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `make fmt: Argument list too long on ALL_SRC shell expansion`
- 1 min: `check-go-version.sh reports mismatches from .tools/go and GOPATH go.mod files that are not part of the repo`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
