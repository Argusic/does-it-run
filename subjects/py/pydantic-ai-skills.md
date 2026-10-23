# pydantic-ai-skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DougTrajano/pydantic-ai-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pydantic-ai-skills

## Pinned environment

- Project commit: `840f217c7b70003be3c2d79d2f2fe8a2532a913f`
- Test commit: `840f217c7b70003be3c2d79d2f2fe8a2532a913f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 48.9 to 48.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 48.9 | 5 | 5 | [run](https://argusic.com/run/51123a47-99a9-4b0c-95dc-f5dbdf2e5ef4) |

## What was observed on a clean machine

Attempt 1:

- 55 min: `Installed latest pydantic-ai-harness 0.59/slim 2.59 changed the Skills contract: construction-time apply yields a placeholder ('skills') because libraries are read in for_run, so every skill_names/catalog test saw ['skills'] and 58 tests fa`
- 2 min: `SkillPackage has no files_empty() attribute from a previous partial patch`
- 3 min: `RunContext slice: Skills.for_run needs ctx.workspace; agent.run without a workspace raises UserError 'Skills needs a workspace'`
- 2 min: `Harness 0.36+ moved frontmatter-name mismatch and overlong-description validation from construction ValueError to for_run UserWarning`
- 1 min: `mypy arg-type error in _render_leaf over the widened instruction union type`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
