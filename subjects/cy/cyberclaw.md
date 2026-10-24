# CyberClaw

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ttguy0707/CyberClaw, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/cyberclaw

## Pinned environment

- Project commit: `12b7c6d52fcc38e134cd0f1aeb7aba420ad23274`
- Test commit: `12b7c6d52fcc38e134cd0f1aeb7aba420ad23274`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.6 to 3.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 3.6 | 1 | 1 | [run](https://argusic.com/run/280f9375-30d3-4e94-8830-01b3437a747e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Mock LLM server launched via nohup backgrounding exited when its parent shell closed; cyberclaw run then failed with connection refused.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
