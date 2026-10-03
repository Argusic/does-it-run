# learn-claude-code

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shareAI-lab/learn-claude-code, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/learn-claude-code

## Pinned environment

- Project commit: `0dcafa2ae053a1ddd6a72f265431104b08a5aa13`
- Test commit: `0dcafa2ae053a1ddd6a72f265431104b08a5aa13`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 5.1 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 5 | 5.8 | 3 | 3 | [run](https://argusic.com/run/f4f4cfec-0771-4852-a578-3f3031cb628f) |
| 2 | pass | 100 | 3 | 5.9 | 1 | 1 | [run](https://argusic.com/run/a29c0c6f-0e75-435f-9236-4418de14980d) |
| 3 | pass with mocks | 92 | 0 | 5.1 | 0 | 0 | [run](https://argusic.com/run/26e4e234-ea63-445a-bcc7-e5b58b1172fe) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pip and python3-venv missing from container`
- 1 min: `No 'python' binary (only python3 available), causing test_goal_loop.py failure`
- `Node.js 18.19.1 too old for Next.js 16 (requires >=20.9.0)`

Attempt 2:

- 1 min: `test_goal_loop.py called 'python' but only 'python3' exists on system`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
