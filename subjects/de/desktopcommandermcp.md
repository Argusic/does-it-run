# DesktopCommanderMCP

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wonderwhy-er/DesktopCommanderMCP, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/desktopcommandermcp

## Pinned environment

- Project commit: `ea8e9a47440ccffefede7060e0ddb490540f414d`
- Test commit: `ea8e9a47440ccffefede7060e0ddb490540f414d`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 9.2 to 42.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 6 | 42.2 | 4 | 4 | [run](https://argusic.com/run/916bc93d-f5de-4932-926a-0184e796e292) |
| 2 | pass | 100 | 5 | 9.2 | 0 | 0 | [run](https://argusic.com/run/b81e4b98-615b-4ae4-a282-8dce8b83e204) |
| 3 | fail | 20 | n/a | 19.6 | 0 | 0 | [run](https://argusic.com/run/d9efaee4-b683-4c9f-b4c0-9492b3e0ce98) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `test-markdown-editor-edit-diff.js: navigator is not defined , prosemirror-view accesses navigator.userAgent at import time`
- 0.1 min: `test-markdown-editor-roundtrip.js: same navigator is not defined error`
- 0.1 min: `test-remote-channel-reconnect.js: Cannot assign to read only property 'now' of '#<Performance>' (Node 18 restriction)`
- 0.2 min: `test-pdf-creation.js: Chrome binary present but cannot launch , missing system libraries (libglib-2.0.so.0, libnss3.so, libcups.so.2, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
