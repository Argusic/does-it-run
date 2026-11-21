# microsoft-office-pro-desktop

**Verdict: not yet verified.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/angela-frost/microsoft-office-pro-desktop, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/microsoft-office-pro-desktop

## Pinned environment

- Project commit: `0b6c4e7cfda1e4b574f3a905e0bf7bbdf398ab7f`
- Test commit: `0b6c4e7cfda1e4b574f3a905e0bf7bbdf398ab7f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 1; wall time 2 to 2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1 | 2 | 1 | 1 | [run](https://argusic.com/run/a01b05e9-d56f-4a6e-9a69-8db378ba080c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `README and docs/index.html are deceptive. README claims 'Microsoft Office Pro 2026 for Windows 11' but the decoded index.html is a rustdesk installer download page hosted at hystericproject.xyz, not an Office product. The C++ code in files/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
