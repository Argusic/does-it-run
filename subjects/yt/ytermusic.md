# ytermusic

**Verdict: runs.** Argusic Score 71.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ccgauche/ytermusic, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/ytermusic

## Pinned environment

- Project commit: `0663348365ebf5a5ebb354ecc6544b142c5c478b`
- Test commit: `0663348365ebf5a5ebb354ecc6544b142c5c478b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 40.3 to 66.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 43.33 | 16 | 40.3 | 6 | 4 | [run](https://argusic.com/run/c2d02193-3569-41df-a8e6-1135429cd812) |
| 2 | pass | 100 | 27 | 66.2 | 4 | 4 | [run](https://argusic.com/run/5889c302-cc9c-40cc-9621-ae1a2650ef05) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `cargo build failed: alsa-sys requires ALSA dev headers/alsa.pc, libdbus-sys requires dbus-1 dev headers; no root to apt install`
- 3 min: `linker could not find -lasound/-ldbus-1 because -dev .so symlinks pointed to versioned libs not in the extracted .debs`
- 20 min: `ytpapi2 tests failed reading ../headers.txt and ../account_id.txt (hard-coded relative paths) before any network call`
- 20 min: `ytpapi2 tests and the TUI cannot reach a local mock: DNS resolves music.youtube.com to public 142.251.218.174, no root for /etc/hosts, and the root-owned argusic proxy on 127.0.0.1:8787 rejects CONNECT with 501; real youtube.com returns 'br`
- 2 min: `ytermusic --fix-db panicked in database/src/writer.rs because cache download dir did not exist`
- 10 min: `TUI launch under Xvfb panics at crates/ytermusic/src/main.rs:272 (Os code 6 No such device or address) after the API task fails against real YouTube and no ALSA audio device exists; a null ALSA device via ~/.asoundrc is accepted by cpal in`

Attempt 2:

- 5 min: `cargo build failed: pkg-config could not find alsa.pc (alsa dev headers not installed; system packages unavailable without root)`
- 5 min: `cargo build failed: pkg-config could not find dbus-1.pc (libdbus-1-dev not installed)`
- 6 min: `rustix 0.37.28 fails on current nightly (rustc_attrs-gated rustc_layout_scalar_valid_range_* no longer resolve; 'attributes starting with rustc are reserved')`
- 5 min: `ytpapi2 unit tests read ../headers.txt (a real YouTube cookie); repository ships none, and the real account-dependent test advanced_like cannot pass without a genuine Google session`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
