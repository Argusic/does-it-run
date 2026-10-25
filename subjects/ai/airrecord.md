# airrecord

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sirupsen/airrecord, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/airrecord

## Pinned environment

- Project commit: `06a65af5f0757192662454a6fa7a466020957eaa`
- Test commit: `06a65af5f0757192662454a6fa7a466020957eaa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.5 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.5 | 7 | 7 | [run](https://argusic.com/run/97ca1627-9a9c-4783-9a38-4843d082ae67) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Ruby not installed in container`
- 1 min: `Shared library libruby-3.2.so.3.2 not found`
- 1 min: `gem/bundler scripts use #!/usr/bin/ruby3.2 shebang not found in PATH`
- 1 min: `rubygems.rb requires rbconfig from arch-specific lib dir`
- 1 min: `libyaml-0.so.2 not found for psych YAML extension`
- 2 min: `Native gem extensions fail: missing ruby.h header for mkmf`
- 1 min: `associations_test.rb uses MiniTest::Test instead of Minitest::Test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
