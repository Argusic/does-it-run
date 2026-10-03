# ai-engineering-from-scratch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rohitg00/ai-engineering-from-scratch, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-engineering-from-scratch

## Pinned environment

- Project commit: `a56b4b8ad43a3767c771953d217036813f697bc7`
- Test commit: `a56b4b8ad43a3767c771953d217036813f697bc7`
- Worker image digests: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`, `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 3.8 to 26 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 26 | 5 | 5 | [run](https://argusic.com/run/504684d1-ba0e-43ef-ad18-1b68c711eef0) |
| 2 | pass | 100 | 0.04 | 3.8 | 0 | 0 | [run](https://argusic.com/run/c74228dd-37e0-4ebd-9358-ea954465eea0) |
| 2 | pass | 100 | 5 | 9 | 3 | 3 | [run](https://argusic.com/run/c8b28e2b-867a-409d-9697-89dc44bd6419) |
| 3 | pass | 100 | 8 | 25.4 | 4 | 4 | [run](https://argusic.com/run/e173057a-9f87-40e1-a802-6d6834f1a69e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 externally-managed-environment prevents system-wide pip install`
- 3 min: `Test files in 13-tools-and-protocols/06,07,08,09 used 'import main' without sys.path setup`
- 4 min: `Test file in 08-building-an-mcp-client had mismatched API (make_request/send/string/response_from don't exist)`
- 5 min: `Test file in 09-mcp-transports had wrong request headers (missing MCP-Protocol-Version, Mcp-Method, and Accept) and wrong _meta keys`
- 1 min: `Test in 39-instruction-tuning-sft had too-tight byte-length assertion (assertLessEqual 4, got 6)`

Attempt 2:

- 2 min: `PEP 668 on Debian blocks system pip install`
- 1 min: `Rust toolchain not pre-installed`
- `Julia not available in container`

Attempt 3:

- 7 min: `pip install failed: externally-managed-environment`
- `rustc not found in container`
- `julia not found in container`
- `Node.js v18.19.1 (verify.ts requires v20+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
