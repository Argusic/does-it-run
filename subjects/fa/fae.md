# fae

**Verdict: runs.** Argusic Score 97.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wearefine/fae, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/fae

## Pinned environment

- Project commit: `b3416fbc44543bc80b83c61a4ff5c5e12771879a`
- Test commit: `b3416fbc44543bc80b83c61a4ff5c5e12771879a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 59 to 59 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 97.14 | 92 | 59 | 7 | 6 | [run](https://argusic.com/run/17028dd7-740f-4802-9064-91e536741c86) |

## What was observed on a clean machine

Attempt 1:

- 22 min: `No Ruby on host; RVM prebuilt Ruby 3.1.1 (Debian 11) had broken openssl.so (needs libssl.so.1.1) and psych.so (needs libyaml); gem/bundler could not run`
- 25 min: `bundler 2.3.7 aborts every install with Bundler::APIResponseMismatchError on loofah-2.22.0 (lockfile entry lacks crass/nokogiri deps the gem really declares)`
- 12 min: `mysql2/pg gems cannot build: host lacks libmysqlclient/libpq dev headers; no root to install libmysqlclient-dev/libpq-dev`
- 8 min: `capybara-webkit (gem from git) cannot build: qmake/Qt5/WebKit absent, no root for libqt5webkit5-dev`
- 14 min: `json 3.0.2 + ddtrace 1.23 (and devise sign-in during requests) crash: unknown keyword quirks_mode`
- 8 min: `rake app:db:migrate duplicated engine migrations (dummy copies AddUserTable etc.) and schema included MySQL-only utf8mb4 collations/check-constraint`
- 3 min: `7 specs fail in clean final run: deploy#index needs Fae.netlify (3rd-party config), Global nav + fae_table_collapse assert JS-collapsed DOM (need real JS driver), helper SVG test needs ImageMagick rsvg-convert delegate missing on host`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
