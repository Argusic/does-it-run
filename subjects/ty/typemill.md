# typemill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/typemill/typemill, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/typemill

## Pinned environment

- Project commit: `dc644958c716ac393c63daeb98891c66eaae8ccd`
- Test commit: `dc644958c716ac393c63daeb98891c66eaae8ccd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17.4 to 21 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 17.4 | 4 | 4 | [run](https://argusic.com/run/e0459860-3fc1-41d7-9c4a-8bd1c01d6246) |
| 2 | pass | 100 | 7 | 21 | 2 | 2 | [run](https://argusic.com/run/93a85691-5d7e-415b-8a7b-793c063870db) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PHP and Composer are not installed in the container and system packages cannot be installed without root`
- 4 min: `Settings::loadSettings() unconditionally set 'setup' => true, so web/api routes never loaded and POST /tm/setup failed with Runtime: Named route does not exist for name: auth.login (500)`
- 3 min: `SecurityMiddleware called routeParser->urlFor('auth.login') on POSTs during setup when that route is not registered, causing the same 500`
- 2 min: `PHP 8.5 deprecations: implicit nullable parameter in Settings::createSettings() and null preg_match subject in Valitron during setup`

Attempt 2:

- 2 min: `PHP and Composer not pre-installed in container`
- 3 min: `PHP built-in server exits after Slim app processes a request due to header() state conflicts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
