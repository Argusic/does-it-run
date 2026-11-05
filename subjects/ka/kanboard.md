# kanboard

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kanboard/kanboard, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/kanboard

## Pinned environment

- Project commit: `cf53b54597b67b60140586c09c2fe6132ead013c`
- Test commit: `cf53b54597b67b60140586c09c2fe6132ead013c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.4 to 59.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 12.4 | 3 | 3 | [run](https://argusic.com/run/7c70adca-ff52-434b-bfed-b6d1c6415a71) |
| 2 | pass | 100 | 58 | 59.8 | 4 | 4 | [run](https://argusic.com/run/94874a6f-5ba1-4bac-ab27-b60e0b0567f2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP binary in container`
- 1 min: `No composer`
- 1 min: `No config.php`

Attempt 2:

- 8 min: `No PHP runtime in container (php: not found)`
- 1 min: `composer.phar would not run: /usr/bin/env: 'php': No such file or directory`
- 45 min: `PHPUnit error: Call to undefined function Kanboard\Group\ldap_escape() (ext-ldap missing)`
- 26 min: `Attempted stock static PHP builds lack ext-ldap; building custom static PHP blocked by GitHub API 403 rate limit and missing build deps (bison/re2c/flex/autoconf/automake/libtool not present, no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
