# wiki

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/frappe/wiki, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/wiki

## Pinned environment

- Project commit: `ccbbe9237b2e6b80269afd4c09471484971dd7ef`
- Test commit: `ccbbe9237b2e6b80269afd4c09471484971dd7ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18 to 18 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 36 | 18 | 8 | 8 | [run](https://argusic.com/run/0c885a5c-627f-4ec9-832c-6b33e2b78aec) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `requires-python = ">=3.14" but container has Python 3.12`
- 1 min: `System Python is externally managed`
- 2 min: `yarn not installed`
- 1 min: `marked@17.0.2 requires Node >=20 (have 18.19.1)`
- 3 min: `@framework/ui link:../../frappe/ui symlink broken (Frappe Framework not available)`
- 5 min: `import.meta.dirname in unplugin-vue-components requires Node >=21.2`
- 2 min: `socket.js imports ../../../../sites/common_site_config.json resolving to /sites/ (no permissions)`
- 2 min: `@framework/ui/telemetry/index.ts and pulse.ts not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
