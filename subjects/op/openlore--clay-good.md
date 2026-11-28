# OpenLore

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/clay-good/OpenLore, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/5caebb85-b87c-449e-ae35-445899268bf2

## Pinned environment

- Project commit: `9ac772057c50d75f672615edd6599c4fc6676b9d`
- Test commit: `9ac772057c50d75f672615edd6599c4fc6676b9d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 56.5 to 56.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 56.5 | 5 | 5 | [run](https://argusic.com/run/5caebb85-b87c-449e-ae35-445899268bf2) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18 cannot run this project (requires Node 22+. node:sqlite is a built-in module only available in Node 22)`
- 8 min: `npm 9 cannot parse 'file:' in overrides (tree-sitter-cli override uses file:stubs/tree-sitter-cli-stub, which npm 9 rejects as an invalid semver comparator)`
- 5 min: `npm 9 skips optionalDependencies requiring Node 20+, leaving vite, @modelcontextprotocol/sdk, @lancedb/lancedb, @vitejs/plugin-react uninstalled`
- 2 min: `tree-sitter prebuilt native addons (.node files) compiled for Node 18 ABI (v109) segfault on Node 22 ABI (v127)`
- `4 test files still crash with SIGSEGV (vitest worker forks use system Node 18, not Node 22, via process.execPath)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
