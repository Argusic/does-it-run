# panel

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Ctrlpanel-gg/panel, licensed MPL-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/panel

## Pinned environment

- Project commit: `b3bd1ed50b9f50b76797d09609980fdb4ae70252`
- Test commit: `b3bd1ed50b9f50b76797d09609980fdb4ae70252`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 57.1 to 80.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 80.9 | 0 | 0 | [run](https://argusic.com/run/741d2708-b6a3-4582-9eb4-64f0dd6daa41) |
| 2 | pass with mocks | 92 | 100 | 57.1 | 10 | 10 | [run](https://argusic.com/run/827bbb4f-5f9b-4693-b0af-fc05bc88b7de) |

## What was observed on a clean machine

Attempt 2:

- 30 min: `No PHP/Composer/MySQL/Redis and no root, so system packages could not be installed`
- 2 min: `composer install failed at package discovery because Redis refused connections`
- 1 min: `Test suite failed because the testing database was empty`
- 5 min: `PHPUnit rejected non-static data providers in four test files`
- 15 min: `TestUserCommand mocked a nonexistent App\Classes\Pterodactyl class`
- 10 min: `User::__construct() silently dropped factory/fill attributes`
- 20 min: `Tests failed with 403 because the removed role column left test users without roles`
- 8 min: `usefullinks store/update threw TypeError on PHP 8 because position was missing`
- 10 min: `Every page returned HTTP 500 because MAIL_HOST=null from .env.example crashes Symfony Mailer during Debugbar boot`
- 1 min: `Root path redirected to /installer without an install marker`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
