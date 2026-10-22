# readmeX

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aibox22/readmeX, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/readmex

## Pinned environment

- Project commit: `782fc3f54b6c79d2beb17e3b2605a5cbc4a9747d`
- Test commit: `782fc3f54b6c79d2beb17e3b2605a5cbc4a9747d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 7.6 | 4 | 4 | [run](https://argusic.com/run/405739f2-f1f0-4b58-a188-a9dc0b3f33a4) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `README's 'gh skill install' command cannot run here: 'gh' binary is not installed in this container`
- 3 min: `System Python is PEP 668 externally-managed, so 'pip install --user mkdocs' failed`
- 1 min: `MkDocs build emitted a warning: docs/index.md links '../../images/logo.svg' which is not a documentation file`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
