# examples

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elevenlabs/examples, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/728ae98e-8995-4c46-841c-4f8d570e489b

## Pinned environment

- Project commit: `9680624d9c7ab58d3f8c427cd11608b2a6027228`
- Test commit: `9680624d9c7ab58d3f8c427cd11608b2a6027228`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 64.2 to 64.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 63 | 64.2 | 5 | 5 | [run](https://argusic.com/run/728ae98e-8995-4c46-841c-4f8d570e489b) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Next.js dev servers hit EMFILE watch errors after many simultaneous dev servers ran, and one music dev server entered a stuck 404 state`
- 6 min: `Four Next.js/Tailwind installs missed the platform binary @tailwindcss/oxide-linux-x64-gnu (pnpm skipped platform optional deps), causing build failure`
- 12 min: `SDK/example code always targets api.elevenlabs.io because examples had no base-URL override; local verification of the real example code paths was impossible without one`
- 12 min: `First mock iteration used a GET-only audio handler that 401'd key validation; TTS example then hit real api.elevenlabs.io`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
