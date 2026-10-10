# northcinder

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cinderline/northcinder, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/northcinder

## Pinned environment

- Project commit: `d1343096a7afff58e0aee4fbf608daf2fa28dc03`
- Test commit: `d1343096a7afff58e0aee4fbf608daf2fa28dc03`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.7 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 18.7 | 4 | 4 | [run](https://argusic.com/run/720a2d66-b537-4195-b879-68e3329ad9d1) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Container Node is v18.19.1 but the workspace requires Node >=20 (site needs >=22.12) and no root/sudo is available to install a system package`
- 3 min: `packages/orders reminder test 'uses the Phoenix buyer-local date' failed under the container's UTC default (expected outcome not_due but code used process-local date)`
- 4 min: `service trust-tranco mtime hot-reload test failed: back-to-back writes get identical mtime on this filesystem, so the lookup saw no change`
- 2 min: `client readme-links test failed: ENOENT /work/repo/AGENTS.md (file absent from the checkout but required by the test)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
