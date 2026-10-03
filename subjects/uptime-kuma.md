# uptime-kuma

**Verdict: runs.** Argusic Score 64 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/louislam/uptime-kuma, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/uptime-kuma

## Pinned environment

- Project commit: `db57bf1106edb1fecfefe73cdd8a682ae66e8e0c`
- Test commit: `db57bf1106edb1fecfefe73cdd8a682ae66e8e0c`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run, no run possible
- Valid runs: 3; wall time 0.5 to 10.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 9 | 10.4 | 4 | 3 | [run](https://argusic.com/run/3460b213-ab89-4f65-85c4-a48afd95acc6) |
| 2 | pass | 85 | 25 | 10.3 | 4 | 1 | [run](https://argusic.com/run/cc1b9e01-4ac2-4d37-935d-4c4f9791d7f9) |
| 3 | fail | 20 | n/a | 0.5 | 0 | 0 | [run](https://argusic.com/run/f1e4c274-da16-4ce1-b8d7-7278995744f0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.19.1 installed, project requires >= 20.4.0`
- 2 min: `unlimited-timeout package is ESM-only but required via require() in server/model/monitor.js`
- 3 min: `cross-env not found (dev dependency)`
- `38/240 backend tests fail: Docker not available for testcontainers (MQTT, MSSQL, MariaDB, MySQL, Oracle, Postgres, RabbitMQ, SNMP), ping command not available`

Attempt 2:

- 6 min: `Node.js 18 (default) below the engine requirement of >=20.4 for the unlimited-timeout@0.1.0 ESM package; require() of ESM module fails at startup`
- `ping binary not available in container; 3 pingAsync tests fail expecting real ping output`
- `No Docker runtime in container; 33 tests requiring testcontainers (MQTT, MSSQL, MySQL, Oracle, Postgres, RabbitMQ, SNMP, migration) cannot start containerized services`
- `Missing @testcontainers/hivemq dev dependency causes migration test module to fail to load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
