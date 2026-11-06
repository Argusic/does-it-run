# aos-ce

**Verdict: runs.** Argusic Score 88.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/unicity-aos/aos-ce, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/aos-ce

## Pinned environment

- Project commit: `af23fd5944195b8fab2dc238304175a8355d0857`
- Test commit: `af23fd5944195b8fab2dc238304175a8355d0857`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4 | 0 | 0 | [run](https://argusic.com/run/6c87839e-41ac-40c1-b570-02c5c5e49142) |
| 2 | pass with mocks | 77 | 5 | 13.8 | 4 | 1 | [run](https://argusic.com/run/8997db62-10cf-4447-a97f-ebd5575f7898) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `install.sh exited 1: Linux host setup incomplete (bwrap missing, /dev/fuse absent, AppArmor userns restriction active) after successfully installing AOS 2026.10.1`
- 1 min: `aos init --yes --offline on a fresh HOME first failed with 'another distro provision is already running: Resource temporarily unavailable (os error 11)' because the first init was still running; rerun succeeded`
- 1 min: `source-built target/debug/aos init failed: bundled runtime inventory astrid missing (plain cargo build produces no release bundle)`
- 1 min: `astrid run LLM request blocked at capsule egress: 'local-egress consent: not approved; request stays blocked (fail-closed)' for endpoint 127.0.0.1:9999; mock server never received the request`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
