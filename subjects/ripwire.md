# ripwire

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/redhat-et/ripwire, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/ripwire

## Pinned environment

- Project commit: `4c10be9d70f7922e4467f6eac74728979bbefd10`
- Test commit: `4c10be9d70f7922e4467f6eac74728979bbefd10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 21.3 to 52.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 50 | 52.2 | 2 | 0 | [run](https://argusic.com/run/878216de-15b5-460f-afe8-6ed23ad93064) |
| 2 | pass | 100 | 16 | 21.3 | 3 | 3 | [run](https://argusic.com/run/5df10c10-d571-4b22-872f-2f20187bfcf7) |

## What was observed on a clean machine

Attempt 1:

- `test/codexdoctorcheck.sh uses xmllint (libxml2-utils), which is not installed and cannot be installed without root`
- `test/a9disclosurecheck.sh expects window="18mo@HEAD" but binary emits window="18mo@HEAD (no churn evidence)" because this is a 1-commit shallow clone with no churn history`

Attempt 2:

- 1 min: `install build OOM-killed at -j4 under LTO - memory-limited container; retried with -j2 and succeeded`
- `xmllint (libxml2-utils) not available - cannot install without root; ~40 test gates report XML well-formedness failures as a result`
- `a9disclosurecheck.sh section A9.6 window= attribute label mismatch (2 failures) - pre-existing test expectation drift against shallow checkout, not a binary defect`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
