# subvert

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aschmelyun/subvert, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/subvert

## Pinned environment

- Project commit: `a23c47df0fa1c672cd4f61c77badb3f159357503`
- Test commit: `a23c47df0fa1c672cd4f61c77badb3f159357503`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 28.8 to 28.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 30 | 28.8 | 4 | 4 | [run](https://argusic.com/run/64badeca-c827-4b24-a76c-00da97fcd576) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `PHP 8+ and composer were absent in the container and no root is available for apt/sudo`
- 5 min: `Composer's ZipDownloader could not extract dist packages because the PHP zip extension and unzip/7z binaries were missing`
- 3 min: `The locked composer packages (nette/schema, nette/utils, league/config) reject PHP 8.3`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
