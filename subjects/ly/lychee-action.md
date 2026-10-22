# lychee-action

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lycheeverse/lychee-action, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/lychee-action

## Pinned environment

- Project commit: `649b0e4890508ea3e11ea6b3ee35ce899a25afd5`
- Test commit: `649b0e4890508ea3e11ea6b3ee35ce899a25afd5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.4 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 2.4 | 3 | 3 | [run](https://argusic.com/run/b0d585aa-c4c0-49d0-a313-0a7f19a0181c) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `Stale lychee/out.md from an earlier local run was re-scanned by the './**/*.md' glob, producing a self-inflicted 404 on the synthetic report URL (harness artifact, not a repo bug)`
- 1 min: `Partial repo copy missing action.yml/license files caused 3 local-file 404s in lychee (harness setup error)`
- 10 min: `fixtures/broken-link.md link https://example.invalid is auto-excluded by lychee 0.24.2 (built-in excludes), so it cannot demonstrate a broken link; repo CI itself uses foo.bar for that`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
