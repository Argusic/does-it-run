# llm-wiki

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Pratiyush/llm-wiki, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/2dbf4d30-ab72-4b07-871f-6ff0cc0d053a

## Pinned environment

- Project commit: `b1088890ee0743810a92577aecad946c6b3eb2d2`
- Test commit: `b1088890ee0743810a92577aecad946c6b3eb2d2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 7.9 | 3 | 3 | [run](https://argusic.com/run/2dbf4d30-ab72-4b07-871f-6ff0cc0d053a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `./setup.sh: Permission denied , all repo shell scripts are committed as mode 100644 (non-executable)`
- 2 min: `setup.sh pip install markdown failed silently on PEP 668 externally-managed Python ('error: externally-managed-environment'); setup still printed Setup complete and exit 0 with markdown missing`
- 1 min: `llmwiki sync converts 0 sources for sessions active within the last 60 min (live-session guard) unless --include-current is passed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
