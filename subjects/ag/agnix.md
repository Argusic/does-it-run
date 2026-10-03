# agnix

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agent-sh/agnix, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/agnix

## Pinned environment

- Project commit: `e557022f0943a010f0dd4a634da4991cfffaf604`
- Test commit: `e557022f0943a010f0dd4a634da4991cfffaf604`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 20 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/ad7c5a53-e2da-4a25-9355-d6d69c2b1390) |
| 2 | pass | 100 | 22.8 | 20 | 4 | 4 | [run](https://argusic.com/run/666f100e-cd99-4ed7-881b-cbbfce5a6335) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `npm install -g failed due to EACCES on /usr/local/lib/node_modules`
- 16.6 min: `Rust toolchain not found (no rustc/cargo)`
- 2 min: `kiro_fixture_inventory test baseline drift: VER-001 info added 1 extra diagnostic per kiro-fix family`
- 0.2 min: `pip install failed due to externally-managed-environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
