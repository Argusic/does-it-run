# eCommerce-Skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nexscope-ai/eCommerce-Skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ecommerce-skills

## Pinned environment

- Project commit: `ee0fb29433d02ccc22e3e6cea9ab4586d49fd42e`
- Test commit: `ee0fb29433d02ccc22e3e6cea9ab4586d49fd42e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 5.1 | 2 | 2 | [run](https://argusic.com/run/ca1c81d5-6e8e-41c9-8e91-c4ef1c653921) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npx skills latest (v1.7.2) requires node >=22.20; node v18.19.1 in container`
- `skills CLI discovered only 100 of 142 skills , 42 SKILL.md files lack required YAML frontmatter`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
