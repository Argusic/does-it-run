# OPNsensePIAWireguard

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FingerlessGlov3s/OPNsensePIAWireguard, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/opnsensepiawireguard

## Pinned environment

- Project commit: `a0b3dad1e45919c7d61b5dd2af2acac2c4ef91a4`
- Test commit: `a0b3dad1e45919c7d61b5dd2af2acac2c4ef91a4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.6 to 26.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 26.6 | 5 | 5 | [run](https://argusic.com/run/08880da0-c09f-4022-9282-06d5e7a85c6e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing Python dependency 'requests'`
- 1 min: `Missing 'netstat' binary (OPNsense/FreeBSD host tool)`
- 1 min: `Missing '/usr/local/sbin/configctl' binary (OPNsense-specific)`
- 1 min: `Unwritable '/usr/local/www/' (OPNsense web root)`
- 10 min: `Script called real PIA endpoints instead of mocks due to DNS: override_dns() uses private IPs (10.1.0.x) that are unrouteable in this container, and plain requests.get() had no proxy`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
