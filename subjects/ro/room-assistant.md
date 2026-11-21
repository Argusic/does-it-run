# room-assistant

**Verdict: runs.** Argusic Score 89.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mKeRix/room-assistant, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/room-assistant

## Pinned environment

- Project commit: `ed9a860e8ca2f481c76f11b66f632a30551d4416`
- Test commit: `ed9a860e8ca2f481c76f11b66f632a30551d4416`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 10.5 to 40.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 40.7 | 2 | 2 | [run](https://argusic.com/run/07418986-92b1-4c64-97b9-f9f83f35dbad) |
| 2 | pass with mocks | 78.67 | 1.5 | 10.5 | 3 | 1 | [run](https://argusic.com/run/5bd58c45-f228-45de-b9cf-d03004dea5b5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Build failed: TS2307 - Cannot find module 'canvas'`
- 5 min: `Test suite failed: Could not locate native binding epoll.node for onoff`

Attempt 2:

- 0.5 min: `Missing optional dependency 'canvas' prevented TypeScript build`
- `GPIO test suites failed - epoll native bindings not available in container (no /dev/gpio or hardware)`
- `mdns native bindings not compiled - libavahi-compat-libdnssd-dev system package missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
