# kms-tools

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ikxin/kms-tools, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kms-tools

## Pinned environment

- Project commit: `28b32ab068da713dd38a3ae87f09fda085a85db0`
- Test commit: `28b32ab068da713dd38a3ae87f09fda085a85db0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.1 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 11.1 | 3 | 3 | [run](https://argusic.com/run/05ee6565-35c0-464a-969d-87653b6e01dc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.19.1 不满足 pnpm 要求的 >=22.13`
- 2 min: `全局 npm install 因 EACCES 权限不足失败`
- 1 min: `pnpm 包装脚本被覆盖导致无法执行`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
