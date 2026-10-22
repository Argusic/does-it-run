# mg

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/troglobit/mg, licensed Unlicense, written in C.

Evidence and recordings: https://argusic.com/subject/mg

## Pinned environment

- Project commit: `7bae32d010515c4d8f5fa927f13058cebc9ee8e6`
- Test commit: `7bae32d010515c4d8f5fa927f13058cebc9ee8e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 10.2 | 3 | 3 | [run](https://argusic.com/run/556d5bd6-5a19-46d1-9ff8-de7aa4989dc7) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `autogen.sh fails: autoreconf not found (no autotools in container)`
- 2 min: `Default curses build cannot compile: /usr/include term.h/curses.h headers absent (no libncurses-dev; cannot apt install without root)`
- 5 min: `Link errors: missing fparseln/recallocarray/strtonum and cscope symbols; lib objects lacked -Isrc`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
