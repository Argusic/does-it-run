# codex-security

**Verdict: runs.** Argusic Score 94.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openai/codex-security, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codex-security

## Pinned environment

- Project commit: `8c78e65532155c713208acab90d66afac55f9a69`
- Test commit: `8c78e65532155c713208acab90d66afac55f9a69`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 14.8 to 58.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 59 | 58.3 | 6 | 6 | [run](https://argusic.com/run/67c453e8-7826-4095-9e69-311353e7337b) |
| 2 | pass | 96.67 | 6 | 14.8 | 6 | 5 | [run](https://argusic.com/run/8a63e64b-1b60-4d5b-9cf8-ac56d066eb57) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 was installed; project requires ^22.13.0`
- 2 min: `pnpm and bun not found`
- 5 min: `Rust toolchain not found (required for native binding)`
- 10 min: `build:plugin failed: missing native prebuilt binaries and license files`
- 5 min: `Default umask 0o002 creates group-writable directories (0775), causing workbench scan-directory permission checks to reject /tmp ancestors`
- 5 min: `test_windows_report_e2e.py and test_nested_target_name_is_a_literal_git_pathspec fail because /tmp/pytest-of-runner/.../scans dirs are group-writable`

Attempt 2:

- 2 min: `Node.js v18.19.1 is too old (requires >=22.13.0)`
- 1 min: `pnpm not available and corepack signature verification failed for pnpm@11.25.0`
- 0.5 min: `Stale /work/repo/.npmrc with prefix=/home/runner/.npm-global prevented npm configuration changes`
- 0.5 min: `Python pip install failed due to externally-managed environment`
- 0.5 min: `bwrap: No permissions to create a new namespace (kernel restriction)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
