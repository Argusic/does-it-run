# Boterdrop-Solver

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/najibyahya/Boterdrop-Solver, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/boterdrop-solver

## Pinned environment

- Project commit: `967d532b1d72a4f3a3f7b07b4374a19fa9365c66`
- Test commit: `967d532b1d72a4f3a3f7b07b4374a19fa9365c66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 3.9 to 16.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 16.9 | 0 | 0 | [run](https://argusic.com/run/4122f92c-6e5e-478c-baa7-4c619fe6dc3f) |
| 2 | pass with mocks | 92 | 0.5 | 3.9 | 2 | 2 | [run](https://argusic.com/run/9b6a4a26-6740-4078-ad55-f74730b5cc3c) |

## What was observed on a clean machine

Attempt 2:

- `playwright install-deps fails without root (su authentication failure)`
- `Actual CAPTCHA solving requires external internet sites (Cloudflare, reCAPTCHA, AWS WAF) to serve real challenges`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
