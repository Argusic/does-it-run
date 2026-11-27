# cherry

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cherry-game/cherry, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/cherry

## Pinned environment

- Project commit: `4a6c56e0d90fd65f616cb7fdc09c14260b2a26fe`
- Test commit: `4a6c56e0d90fd65f616cb7fdc09c14260b2a26fe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23 to 23 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 23 | 7 | 7 | [run](https://argusic.com/run/b4a4194e-ed76-400e-b7f8-8fb9ffefe3c9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.24+ not installed in environment`
- 2 min: `extend/snowflake: TestNewNode used node=5000 but NodeBits=16 gives nodeMax=65535, so 5000 is valid. Test expected error that never came.`
- 2 min: `extend/snowflake: TestUnmarshalJSON compared errors with != operator but JSONSyntaxError contains a []byte field (not comparable), causing panic`
- 1 min: `extend/snowflake: TestBase58 and TestBase36 used invalid-expected strings that were actually valid in those encodings`
- 1 min: `extend/mapstructure: Example tests expected output from package 'mapstructure' but package is named 'cherryMapStructure'`
- 1 min: `extend/reflect: TestGetFuncName passed a struct pointer to GetFuncName which panics with 'not func type'`
- 2 min: `net/nats: ReleaseNatsMsg used clear() on shared header map, mutating caller's header`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
