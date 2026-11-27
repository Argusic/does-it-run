# scriptc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel-labs/scriptc, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/scriptc

## Pinned environment

- Project commit: `05021faf2ffa6bdd9cc6529f9321ef726219a830`
- Test commit: `05021faf2ffa6bdd9cc6529f9321ef726219a830`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.9 to 25.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 25.9 | 4 | 4 | [run](https://argusic.com/run/402e85d4-32d9-4b51-b8d9-582730e88c44) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18 installed but project requires 24+; pnpm not found`
- 13 min: `LLVM native helper binary missing: /work/repo/packages/llvm-linux-x64-gnu/bin/scriptc-llvm-codegen does not exist , SC3003 error on any compile`
- 8 min: `Runtime pack missing: @scriptc/runtime-linux-x64-gnu had no artifacts dir or runtime-pack.json , SC3003 error after LLVM helper was fixed`
- 1 min: `clang not on PATH: linker failed with ENOENT when trying to link final executable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
