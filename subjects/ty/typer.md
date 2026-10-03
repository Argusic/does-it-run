# typer

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fastapi/typer, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/typer

## Pinned environment

- Project commit: `82b83959d9e900215ed8ff2a56a766ff066e1c75`
- Test commit: `82b83959d9e900215ed8ff2a56a766ff066e1c75`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 6.8 to 19.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 6.8 | 1 | 1 | [run](https://argusic.com/run/66b50f25-8da5-4687-a848-35a80a81cc69) |
| 2 | pass | 100 | 7 | 19.9 | 1 | 1 | [run](https://argusic.com/run/9f88f110-cfaf-4626-88e1-41a184d85dae) |
| 3 | fail | 20 | n/a | 18.8 | 0 | 0 | [run](https://argusic.com/run/2af25fd8-f101-46a4-802f-4df186849e94) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Container has NO_COLOR=1 and TERM=dumb, suppressing Rich ANSI output. Two printing-tutorial tests (test_tutorial001::test_cli, test_tutorial002::test_cli) failed because normalize_rich_output found no ANSI codes to replace.`

Attempt 2:

- 10 min: `Tests test_tutorial001 and test_tutorial002 failed due to Rich 15.0.0 behavior change: Console(force_terminal=True) without explicit color_system emits no ANSI codes, and NO_COLOR=1 env var was set`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
