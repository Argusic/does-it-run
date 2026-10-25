# dockside

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/newsnowlabs/dockside, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/dockside

## Pinned environment

- Project commit: `c5834215605e4230f9c1f6b576fd8f49b5a71629`
- Test commit: `c5834215605e4230f9c1f6b576fd8f49b5a71629`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.5 to 13.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 13.5 | 4 | 4 | [run](https://argusic.com/run/35752eac-e165-45b8-9259-655118270753) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Missing Perl modules (JSON, Try::Tiny, URI, Expect, Mojolicious, IO::Async, Crypt::Rijndael, Term::ReadKey, YAML::LibYAML, IO::Pty, Future) , none installed in base container`
- 1 min: `Missing shellcheck binary`
- 1 min: `test.sh install step for Perl deps tried apt-get install without root (E: Could not open lock file)`
- 1 min: `pip install ./cli creates entry point 'dockside_cli' but source file is named 'dockside', causing ModuleNotFoundError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
