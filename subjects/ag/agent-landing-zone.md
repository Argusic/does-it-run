# agent-landing-zone

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Azure/agent-landing-zone, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agent-landing-zone

## Pinned environment

- Project commit: `9a0243b282d6df97683e8b24d17006366d9fbc69`
- Test commit: `9a0243b282d6df97683e8b24d17006366d9fbc69`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 22 | 5.1 | 4 | 4 | [run](https://argusic.com/run/8c255909-4f2c-4fae-aaa3-bb0bf1b2f330) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip could not satisfy both config/requirements.txt (azure-identity==1.25.3) and util/requirements.txt (azure-identity==1.23.0) in one install command`
- 2 min: `Initial hosted composition CLI failed with DeploymentTopologyError because the (default) hosted-no-panel topology requires HOSTED_AGENT_RESOURCE_SCOPE`
- 4 min: `Real private-network/TLS probe cannot be satisfied: container DNS cannot resolve Azure public endpoints (cfg.azconfig.io NXDOMAIN) and no RFC1918 DNS/VPN is available`
- 1 min: `sh -n reported syntax error in bash-shebang hooks`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
