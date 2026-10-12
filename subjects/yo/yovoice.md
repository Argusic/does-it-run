# yovoice

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leemysw/yovoice, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/yovoice

## Pinned environment

- Project commit: `b065b665267969cb51dab6af8c2a35f1923caeab`
- Test commit: `b065b665267969cb51dab6af8c2a35f1923caeab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.9 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 9.9 | 3 | 3 | [run](https://argusic.com/run/284d3401-539f-4825-96c2-fe51931b2d01) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `go 不在 PATH（需要 Go 1.26+），系统 Node 18.19 低于要求的 22+，且无 pnpm`
- 4 min: `容器无中文字体，中文界面渲染成空白导致 7 个 Playwright 用例超时/几何断言失败`
- 2 min: `全量并发跑测试时 7 个用例偶发超时失败（67 过/7 失败、64 过/10 失败）`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
