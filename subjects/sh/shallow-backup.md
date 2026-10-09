# shallow-backup

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alichtman/shallow-backup, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/shallow-backup

## Pinned environment

- Project commit: `8fc823481d58c76b804e0ccf2d55c9777b76f65d`
- Test commit: `8fc823481d58c76b804e0ccf2d55c9777b76f65d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 4.8 | 4 | 4 | [run](https://argusic.com/run/e42405d0-8d0b-4b4e-9907-f1a594041475) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Interactive git remote URL prompt crashes in non-TTY (headless/CI) environments with termios error`
- 1 min: `git_set_remote crashes on unreachable remote URLs (fetch fails)`
- 1 min: `install_trufflehog_git_hook calls sys.exit() when trufflehog/pre-commit are missing`
- 1 min: `trufflehog package dependency conflict with GitPython , trufflehog pins GitPython==3.0.6 but shallow-backup requires >=3.1.20`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
