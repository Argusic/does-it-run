# nanzi-ai-agent-platform

**Verdict: runs with mocks.** Argusic Score 61 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RandyChen1985/nanzi-ai-agent-platform, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/nanzi-ai-agent-platform

## Pinned environment

- Project commit: `5cdaf541843764c2c79e30fdb4bfe4edd1e6710f`
- Test commit: `5cdaf541843764c2c79e30fdb4bfe4edd1e6710f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 28.2 to 34.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 35 | 28.2 | 4 | 0 | [run](https://argusic.com/run/bb38a7cf-f68c-4d5e-bc6b-8ea9bd7e767d) |
| 2 | pass with mocks | 92 | 4.5 | 34.9 | 3 | 3 | [run](https://argusic.com/run/0bff4bdd-538f-43c3-94df-32d4cb0073fd) |

## What was observed on a clean machine

Attempt 1:

- `Python 3.11 在容器中不可用，使用系统 Python 3.12.3，项目代码兼容运行`
- `Node.js 18.19.1 不满足 Vite 7 前端构建要求（需 20.19+），前端无法编译`
- `容器中无 MySQL/Redis Stack/PostgreSQL/Docker 服务，服务无法启动`
- 5 min: `11 个 apply-sql-native.sh 测试因缺少 mysql/psql 命令行客户端而失败`

Attempt 2:

- 5 min: `Node.js v18.19.1 不支持 Vite 7 所需的 >=20.19.0 版本，导致前端构建失败`
- `容器内无 MySQL 服务, , 数据库部分需要 MySQL 8.0+ 或 PostgreSQL 14+`
- `容器内无 Redis Stack 服务, , 需要支持 RediSearch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
