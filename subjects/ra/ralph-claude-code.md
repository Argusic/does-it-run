# ralph-claude-code

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/frankbria/ralph-claude-code, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/ralph-claude-code

## Pinned environment

- Project commit: `e8533cc3f00900e6f3f4acf8c8761e1db4a26e47`
- Test commit: `e8533cc3f00900e6f3f4acf8c8761e1db4a26e47`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 0.5 | 13 | 2 | 1 | [run](https://argusic.com/run/4833fe3c-670e-4d06-8aaa-e0ccc6b2db4f) |

## What was observed on a clean machine

Attempt 1:

- `ralph-setup --help treats --help as a project name instead of showing help`
- 1 min: `ralph-setup requires git user.name/user.email to be configured (non-interactive git commit fails without them)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
