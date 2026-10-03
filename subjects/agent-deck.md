# agent-deck

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/asheshgoplani/agent-deck, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/agent-deck

## Pinned environment

- Project commit: `3d7cb43acf1bb4a98a5b90d7ca5569061197b7ad`
- Test commit: `3d7cb43acf1bb4a98a5b90d7ca5569061197b7ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 29 to 62.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 29 | 29 | 4 | 4 | [run](https://argusic.com/run/2ff25a36-42d4-4645-85ec-b2ce77b4fd90) |
| 2 | pass | 100 | 37 | 62.1 | 3 | 3 | [run](https://argusic.com/run/619eec31-2d39-44a1-a5b9-71fb5e12d8b2) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `tmux not found in container: systemd-run --user bus not available, tmux library dependencies missing (libutempter, libevent, libncursesw, libtinfo)`
- `Session test TestPersistence_TmuxDiesWithoutUserScope failed: cannot start tmux inside fake login scope , no systemd user bus in container`
- `Tmux service tests (TestStart_Service_SuccessPath) failed: systemd-run --user requires systemd bus not available in container`
- `Web keepalive tests (TestWSKeepalive*) failed: tmux attach-session bridge cannot attach client without PTY/systemd support`

Attempt 2:

- 2 min: `Go compiler not installed`
- 1 min: `tmux not installed`
- 3 min: `TestWSKeepaliveReapsDeadPeer and TestWSKeepaliveHealthyClientSurvives fail in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
