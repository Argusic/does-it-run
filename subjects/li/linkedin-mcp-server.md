# linkedin-mcp-server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/stickerdaniel/linkedin-mcp-server, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/linkedin-mcp-server

## Pinned environment

- Project commit: `f410bfdc32569f8763fde11338b24ec6a0797f0d`
- Test commit: `f410bfdc32569f8763fde11338b24ec6a0797f0d`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 23 to 50.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 2 | 50.7 | 7 | 4 | [run](https://argusic.com/run/5251a87b-7671-4c3c-9365-e1bd113a4cb4) |
| 1 | pass with mocks | 92 | 0.7 | 30.4 | 1 | 1 | [run](https://argusic.com/run/11377424-8c47-4133-96b6-442e7ff9ac3c) |
| 2 | pass with mocks | 92 | 22 | 23 | 6 | 6 | [run](https://argusic.com/run/6e7eb8bb-a98e-4a20-94f7-e855c6f6ea0e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Test failures due to TERM=dumb causing rich console is_dumb_terminal=True which skips progress bar tests`
- 5 min: `Test failures due to Docker runtime policy causing early return in background setup and auto-import tests`
- 1 min: `browser_security test failure: umask 0o02 causes intermediate dirs to get 0o775 instead of expected 0o755`
- 2 min: `browser_driver test failure: container runtime adds WebGL args unconditionally, failing 'args not in launch_options' assertion`
- 10 min: `Chromium cannot launch: missing system shared libraries (libglib, libnss, libx11, etc.) , cannot install without root`
- 2 min: `process_tree test: container process group semantics differ from expectations`
- 1 min: `daemon_election test: process group test fails in container`

Attempt 1:

- 20 min: `Test test_slow_profile_ownership_cannot_block_the_deadline fails in container environments because it doesn't call initialize_bootstrap('managed') before start_background_browser_setup_if_needed. In a container, runtime policy defaults to D`

Attempt 2:

- 1 min: `uv not found in container, had to install it`
- 1 min: `System Python 3.12.3 below project minimum of 3.12.4`
- `6 TestCliProgress tests fail due to rich 15.0.0 API change (Console.quiet attribute, _check_buffer OSError handling)`
- `test_harden_linkedin_tree_noop_outside_linkedin fails: expected mode 0o755 (493) but got 509 (0o775)`
- `test_no_proxy_leaves_webrtc_alone fails: launch_options now includes 'args' key with WebGL flags by default`
- `8 tests fail due to container environment (no libglib for Chromium, Docker detection, process group constraints)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
