# luya

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/luyadev/luya, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/luya

## Pinned environment

- Project commit: `7960f23c71534fac4b24d85083631b2d91ae8c9a`
- Test commit: `7960f23c71534fac4b24d85083631b2d91ae8c9a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 12.9 to 22 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 22 | 5 | 5 | [run](https://argusic.com/run/4f18a1a6-ffa5-4b52-97f3-7847afa155d5) |
| 2 | pass with mocks | 92 | 6 | 12.9 | 5 | 5 | [run](https://argusic.com/run/9101f71b-ca3a-4257-862d-c24e319a530f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP binary missing in container (no root to apt-install)`
- 8 min: `MySQL/MariaDB absent; tests need mysql at 127.0.0.1:8888`
- 4 min: `Access denied for 'root'@'localhost' (using password: YES): Yii PDO connected via localhost host while grants were for 127.0.0.1`
- 3 min: `HealthControllerTest fails with 'public_html/storage: directory exists already' after any prior health run (test asserts fresh-dir state)`
- 3 min: `FormatterTest::testDefaultSettingsFromGivenArray fails: expected 2017/2017/2017 got 2017201720172017/2017201720172017/2017201720172017`

Attempt 2:

- 2 min: `PHP not found in container`
- 1 min: `Composer not found in container`
- 1 min: `intl extension missing in PHP 8.2.10 build`
- 1 min: `HealthControllerTest fails when storage dir exists`
- 2 min: `NextPrevModelTest missing admin_auth table for SQLite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
