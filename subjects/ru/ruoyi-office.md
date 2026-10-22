# ruoyi-office

**Verdict: not yet verified.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yuqing2026/ruoyi-office, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/ruoyi-office

## Pinned environment

- Project commit: `ad56d726368d8c321644d47898a76d3e86f1b548`
- Test commit: `ad56d726368d8c321644d47898a76d3e86f1b548`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 41.2 to 41.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 36 | 41.2 | 5 | 5 | [run](https://argusic.com/run/3916bd36-41ad-4a30-b3de-3e9030535581) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `JDK 21 cacerts trust store empty due to incomplete .deb extraction`
- `CrmContractStatusListener/CrmReceivableStatusListener: getStatus() method not found on BpmProcessInstanceStatusEvent`
- `DesensitizeTest expected '芋***' but got '宇***'`
- `Websocket module fails to compile without provided-scope tenant dependency`
- `MySQL process killed between shell invocations preventing app launch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
