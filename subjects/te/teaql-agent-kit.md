# teaql-agent-kit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/teaql/teaql-agent-kit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/teaql-agent-kit

## Pinned environment

- Project commit: `e0db10da45a4b801f996faf22cd25e1bd52518f6`
- Test commit: `e0db10da45a4b801f996faf22cd25e1bd52518f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0 | 2.4 | 0 | 0 | [run](https://argusic.com/run/9a5752b2-aea8-4625-9212-03160f9b3b72) |
| 2 | pass | 100 | 0.5 | 3.4 | 2 | 2 | [run](https://argusic.com/run/b4db8611-8e2f-46a2-8d29-24a4b99a418c) |

## What was observed on a clean machine

Attempt 2:

- `npx skills add fails: Node.js v18.19.1 too old, needs >=22.20.0 (styleText not found in node:util)`
- `Rust, Java, Go, Swift, C#/.NET toolchains not installed in container, generated-application verification not possible`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
