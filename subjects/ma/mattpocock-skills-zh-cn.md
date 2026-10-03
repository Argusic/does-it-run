# mattpocock-skills-zh-CN

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vinvcn/mattpocock-skills-zh-CN, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/mattpocock-skills-zh-cn

## Pinned environment

- Project commit: `3f92a83668ef8f303e6278f31c49fed9543cbc51`
- Test commit: `3f92a83668ef8f303e6278f31c49fed9543cbc51`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.2 to 15.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 15.2 | 5 | 5 | [run](https://argusic.com/run/31a68a29-817f-4d8d-814a-8bcf23cf1e66) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `SKILL_NAMES array in rewrite-references.mjs had 35 entries but source has 38 skills (3 in-progress skills implement-spec, pr, retro were missing)`
- 0.5 min: `EXPECTED_SKILLS in verify.mjs was 35 but 38 built`
- 0.5 min: `Test assertions expected 35 candidates but got 38`
- 0.5 min: `package.json description said 35 skills but has 38`
- 1 min: `grill-me SKILL.md body had 'grilling' without leading slash so the cross-skill reference rewriter could not prefix it to zh-grilling`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
