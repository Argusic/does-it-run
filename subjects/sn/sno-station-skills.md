# sno-station-skills

**Verdict: runs with mocks.** Argusic Score 85.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sno-ai/sno-station-skills, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/sno-station-skills

## Pinned environment

- Project commit: `0451ca25ab9c70aac62162becbec9a4e1e936d56`
- Test commit: `0451ca25ab9c70aac62162becbec9a4e1e936d56`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 9.5 to 68.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 78.67 | 69 | 68.8 | 3 | 1 | [run](https://argusic.com/run/e0372f83-3ad4-4bf8-b0a5-bcff53c5b6c3) |
| 2 | pass with mocks | 92 | 15 | 9.5 | 3 | 3 | [run](https://argusic.com/run/05f6fd9e-b7f1-4f63-ad7a-5f30a6979b2c) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `medic self-test requires real tmux on /usr/bin:/bin (test hardcodes PATH); tmux not installed and no root`
- 8 min: `rem-reflect selftest-guard requires strace on /usr/bin:/bin in the traced child (hardcoded PATH); strace absent`

Attempt 2:

- 2 min: `tmux not installed - medic test needed it for fixture`
- 2 min: `Python yaml module missing for cross-vendor-security-audit and tag-team self-tests`
- 1 min: `sno-reach state directory missing - onboarding verify mail test failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
