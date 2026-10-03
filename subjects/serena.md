# serena

**Verdict: runs.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oraios/serena, licensed NOASSERTION, written in Python.

Evidence and recordings: https://argusic.com/subject/serena

## Pinned environment

- Project commit: `813fd98f4fd32e0606cb52281467fc055e45a356`
- Test commit: `813fd98f4fd32e0606cb52281467fc055e45a356`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 11.7 to 34.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 11.7 | 0 | 0 | [run](https://argusic.com/run/e182da1a-132c-4bef-be86-34669621d870) |
| 2 | pass with mocks | 72 | 33 | 34.2 | 3 | 0 | [run](https://argusic.com/run/cf821ee1-aded-482b-8c5e-c1d708eba302) |
| 3 | pass with mocks | 92 | 2.5 | 18.9 | 1 | 1 | [run](https://argusic.com/run/4e583e46-35af-41ae-9414-7712a0ee75ac) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Go language server tests fail: Go runtime not installed (no root access to install packages)`
- 10 min: `Pyright LSP tests time out at 60s waiting for workspace analysis; pyright-langserver started via 'uvx --from pyright==1.1.403' hangs on empty temp test directories`
- 5 min: `solidlsp tests for ~40+ languages require language servers (java, rust, typescript, etc.) not available in container`

Attempt 3:

- 5 min: `test_index_with_explicit_language and test_index_with_language_auto_creates timed out because pyright-langserver (downloaded on demand via uvx) exceeded the test's 5-second timeout in an empty directory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
