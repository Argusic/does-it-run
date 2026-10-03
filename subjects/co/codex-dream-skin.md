# Codex-Dream-Skin

**Verdict: could not verify.** Argusic Score 40 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Fei-Away/Codex-Dream-Skin, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/codex-dream-skin

## Pinned environment

- Project commit: `34335d27d54300eccb325cc652f6c93fef428b84`
- Test commit: `34335d27d54300eccb325cc652f6c93fef428b84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.7 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 15 | 4.7 | 2 | 0 | [run](https://argusic.com/run/80556f29-32be-4d9e-b052-0938fb52dfda) |
| 2 | fail | 50 | 0 | 5.8 | 0 | 0 | [run](https://argusic.com/run/4d86ca9b-0152-4c15-8194-1fda6e28fad2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `macos/tests/theme-import-identity.test.sh: /usr/bin/stat -f '%z' uses BSD syntax not available on Linux; also requires /usr/bin/zip and calls macOS-specific import-theme-zip-macos.sh`
- 2 min: `macos/tests/theme-zip-extract.test.sh: missing /usr/bin/zip, /usr/sbin/mkfile, and /usr/bin/jot (macOS-specific tools); calls macOS-specific extract-theme-zip-macos.sh`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
