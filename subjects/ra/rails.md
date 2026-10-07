# rails

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rails/rails, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/rails

## Pinned environment

- Project commit: `4658033fa3b391ab8a928994e12a30257a0afa22`
- Test commit: `4658033fa3b391ab8a928994e12a30257a0afa22`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 53.7 to 53.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 53.7 | 6 | 6 | [run](https://argusic.com/run/a0766516-675b-43fe-8c8e-cb04b9d5b764) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `Ruby 3.2.3 was installed but Rails 8.2 requires Ruby >= 3.3.5`
- 10 min: `Ruby 3.3.9 was initially built with --with-out-ext, missing zlib, psych C extensions`
- 5 min: `Zlib development headers missing for Ruby 3.3.9 build`
- 10 min: `Libxml-ruby gem failed to build native extension due to GCC -Wimplicit-function-declaration warning treated as error`
- 5 min: `Bundled psych 5.2.6 failed extconf despite system yaml being available`
- 2 min: `mysql2, pg, trilogy gems require database server connections`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
