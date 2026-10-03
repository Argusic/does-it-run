# pivpn

**Verdict: could not verify.** Argusic Score 17.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pivpn/pivpn, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/pivpn

## Pinned environment

- Project commit: `aa96de7d27bfe4b9b00b8abe8fda80bb8e2bb81b`
- Test commit: `aa96de7d27bfe4b9b00b8abe8fda80bb8e2bb81b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 16 to 24.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 16 | 16 | 1 | 1 | [run](https://argusic.com/run/be783be6-0025-4575-91b0-fae26a2898c4) |
| 2 | fail | 15 | 0 | 24.1 | 4 | 3 | [run](https://argusic.com/run/b817fb97-7b32-4e7f-8494-f35bedb8c7d9) |

## What was observed on a clean machine

Attempt 1:

- `Root access required: install.sh refuses to run because sudo is not installed and EUID is not 0. Cannot use apt-get to install dependencies (bind9-dnsutils, grepcidr, whiptail, net-tools, bsdmainutils, bash-completion, wireguard-tools, qren`

Attempt 2:

- `Cannot run install script without root - no sudo available`
- `Missing dependencies: wireguard-tools, openvpn, bind9-dnsutils, whiptail, grepcidr, net-tools, bsdmainutils, bash-completion, qrencode - none can be installed without root apt-get`
- `Cannot install shellcheck from apt (no root), downloaded static binary instead`
- `Test suite (ciscripts/test.sh, ciscripts/test_install.sh) requires root and systemd - not runnable here`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
