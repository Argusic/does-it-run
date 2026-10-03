# Explo

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LumePart/Explo, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/explo

## Pinned environment

- Project commit: `521aad4afecedcee689504bac660b5c1e7c465b7`
- Test commit: `521aad4afecedcee689504bac660b5c1e7c465b7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 11.5 to 15.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 15.3 | 4 | 4 | [run](https://argusic.com/run/480e0e7d-aa67-4811-a805-655a1445c17e) |
| 2 | pass with mocks | 92 | 3 | 11.5 | 3 | 3 | [run](https://argusic.com/run/52d93071-6d16-4266-8bd1-8c0676f3778e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in environment`
- 3 min: `Node.js version 18 is too old (requires >= 20 for Vite 6)`
- 1 min: `Native binding missing for @tailwindcss/oxide (npm bug with optional deps)`
- 1 min: `ytmusicapi Python module missing`

Attempt 2:

- 1 min: `No Go compiler installed in container`
- 1 min: `Frontend dist/ directory missing; go:embed requires it`
- 1 min: `TailwindCSS native binding (@tailwindcss/oxide) not resolved by npm`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
