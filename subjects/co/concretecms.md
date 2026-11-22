# concretecms

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/concretecms/concretecms, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/concretecms

## Pinned environment

- Project commit: `bf2747aab53b5335ec7723f127922a0178b5c249`
- Test commit: `bf2747aab53b5335ec7723f127922a0178b5c249`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 14.8 to 33 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 14.8 | 3 | 3 | [run](https://argusic.com/run/ed255a4d-85b7-49d0-b429-e6a1e5a2cae6) |
| 2 | pass | 100 | 32.4 | 33 | 8 | 8 | [run](https://argusic.com/run/65477cbf-712b-4365-be91-91dc37a26395) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No PHP or Composer in container (no root, no apt; sudo absent)`
- 4 min: `composer install failed: Composer new-version advisories block locked league/flysystem 1.1.10 and enshrined/svg-sanitize 0.22.0, plus config.platform php=7.3 makes locked twig/twig 3.11.3 seem uninstallable`

Attempt 2:

- 1.5 min: `PHP and Composer not installed in container`
- 1.5 min: `ext-intl missing from common PHP static build, blocking laminas/laminas-i18n dependency`
- 3 min: `Composer install blocked by security advisories (PKSA-*) and platform.php=7.3 version mismatch for twig/twig`
- 15 min: `No MySQL/MariaDB server available`
- 2 min: `MariaDB listening on port 3307 but test config expected default 3306 with a socket`
- 1 min: `DatabaseTest::testValidConnection didn't pass port to createConnection(), causing connection refused`
- 1 min: `MinPHPVersionTest expected config.platform.php to be '7.3' but it was '8.3.32'`
- 0.5 min: `ExecutableFilesTest detected run_tests.py artifact as executable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
