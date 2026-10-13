# hue

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dominikmartn/hue, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/hue

## Pinned environment

- Project commit: `a910e31cd24b45b9455c0c3502150413aa5a3b32`
- Test commit: `a910e31cd24b45b9455c0c3502150413aa5a3b32`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 2.8 | 3 | 3 | [run](https://argusic.com/run/5a0f6522-ad23-4421-948c-2de2fabc6497) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `js-yaml rejects SKILL.md as one YAML stream (frontmatter + body are one file, expected)`
- 1 min: `generated sample SKILL.md missing literal 'NEVER trigger automatically' → 1 error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
