# paper-age

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/matiaskorhonen/paper-age, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/paper-age

## Pinned environment

- Project commit: `7ca504ad057d7d8915f0b4338678f55d3b5fc668`
- Test commit: `7ca504ad057d7d8915f0b4338678f55d3b5fc668`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.7 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.5 | 3 | 3 | [run](https://argusic.com/run/32c38276-5bdd-4ac4-a49b-6ebf1d0b6709) |
| 2 | pass | 100 | 2 | 4.7 | 1 | 1 | [run](https://argusic.com/run/4fa3a678-5b38-4f12-9b1b-fc274bc80fbf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `cargo not found`
- 1 min: `rpassword needs /dev/tty`
- 1 min: `no zbar shared library for pyzbar`

Attempt 2:

- 1 min: `rpassword::prompt_password fails with 'No such device or address (os error 6)' in headless container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
