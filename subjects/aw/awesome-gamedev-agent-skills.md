# awesome-gamedev-agent-skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gamedev-skills/awesome-gamedev-agent-skills, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/awesome-gamedev-agent-skills

## Pinned environment

- Project commit: `184b72be02884f782a0058f2eeae2ce4277453e4`
- Test commit: `184b72be02884f782a0058f2eeae2ce4277453e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 2.9 | 2 | 2 | [run](https://argusic.com/run/9efe521a-d3ef-470e-8251-9a1815f4fae1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `README quick-start needs Node.js >=22.20, but the container has Node v18.19.1; npx skills crashed with SyntaxError: node:util has no export named styleText`
- 1 min: `5 of 183 tests skipped because Pillow was not installed (asset-tool tests), and pip install of the skill's requirements was blocked by PEP 668 externally-managed environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
