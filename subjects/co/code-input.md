# code-input

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WebCoder49/code-input, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/code-input

## Pinned environment

- Project commit: `eaee4280792a19714304471ab0b0c449b10e3fda`
- Test commit: `eaee4280792a19714304471ab0b0c449b10e3fda`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0 | 4.3 | 3 | 3 | [run](https://argusic.com/run/8912c8c6-c010-4512-b6c7-a932f1a4f356) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `No system browser available (chromium/firefox not installed); repo tests are browser-based with confirm() popups`
- 2 min: `Playwright latest requires Node>=20 but container has Node 18.19.1`
- 3 min: `Autocomplete 'Popup Clickable' test timed out without a human clicking the popup button`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
