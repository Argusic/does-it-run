# textbringer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shugo/textbringer, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/textbringer

## Pinned environment

- Project commit: `8fe81059e70787a1fa2ea0ae10c8790a278d7b98`
- Test commit: `8fe81059e70787a1fa2ea0ae10c8790a278d7b98`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 55.4 to 55.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 57 | 55.4 | 3 | 3 | [run](https://argusic.com/run/770f9827-f2d8-4a85-9dcd-cfe2f109102a) |

## What was observed on a clean machine

Attempt 1:

- 35 min: `No Ruby in container and no root for apt; Ruby 3.2 Ubuntu debs lacked runtime shared libs and ncurses headers were missing.`
- 12 min: `bundle install failed building fiddle (no ffi.h, no libffi.so.8.1.4) and curses (no-PIC ncurses archives rejected when linking shared objects).`
- 10 min: `2 test errors: Prism 2.0 token type splits (BRACE_LEFT_HASH, PARENTHESIS_LEFT_GROUPING) made RubyMode indentation raise 'Unmatched def'.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
