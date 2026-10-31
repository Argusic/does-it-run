# aerospike-client-nodejs

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aerospike/aerospike-client-nodejs, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/aerospike-client-nodejs

## Pinned environment

- Project commit: `e64dca8645265de9f1c9fb697304296f0342474d`
- Test commit: `e64dca8645265de9f1c9fb697304296f0342474d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.1 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 15.1 | 8 | 8 | [run](https://argusic.com/run/05c6a230-305b-45d6-ab5d-e903adf1a2d5) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `C client submodule not initialized`
- 0.5 min: `zlib.h missing (zlib1g-dev not installed)`
- 0.3 min: `yaml.h missing (libyaml-dev not installed)`
- 2 min: `Static libz.a and libyaml.a built without -fPIC, cannot link into shared .node`
- 0.3 min: `binding.gyp uses -lz/-lyaml which need linker search paths; patched to absolute paths`
- 0.5 min: `ESM-only chai v6 incompatible with require()`
- 0.5 min: `ESM-only p-throttle v8 incompatible with require()`
- 0.3 min: `ESM-only chai-as-promised v8 incompatible with require()`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
