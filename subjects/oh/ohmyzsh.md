# ohmyzsh

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ohmyzsh/ohmyzsh, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/ohmyzsh

## Pinned environment

- Project commit: `9112b53fa8b5ab556c7c893aa8be8a247ac512a0`
- Test commit: `9112b53fa8b5ab556c7c893aa8be8a247ac512a0`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14.4 to 14.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass with mocks | 92 | 10 | 14.4 | 3 | 3 | [run](https://argusic.com/run/2c493396-d7ee-48a4-a101-d482bfafad91) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `zsh not installed in container: no zsh binary in PATH or system`
- 1 min: `zsh -n syntax check fails on certain plugins (zsh-interactive-cd, zsh-navigation-tools) because module_path not set for no-exec mode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
