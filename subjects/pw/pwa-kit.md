# pwa-kit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SalesforceCommerceCloud/pwa-kit, licensed BSD-3-Clause, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/pwa-kit

## Pinned environment

- Project commit: `5762377b6ab3779561c3b8223e168d945b314f67`
- Test commit: `5762377b6ab3779561c3b8223e168d945b314f67`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 58.6 to 58.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 58.6 | 2 | 2 | [run](https://argusic.com/run/51ead1f5-e109-480e-a74e-89a0c46accdc) |

## What was observed on a clean machine

Attempt 1:

- `commerce-sdk-react: ShopperBaskets/mutation.test.ts has 2 pre-existing timing failures where customerBaskets.data is undefined instead of expected object`
- `commerce-sdk-react: ShopperBasketsV2/mutation.test.ts has 1 pre-existing timing failure (same root cause)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
