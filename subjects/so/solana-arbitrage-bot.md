# Solana-Arbitrage-Bot

**Verdict: runs with mocks.** Argusic Score 46 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ChangeYourself0613/Solana-Arbitrage-Bot, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/solana-arbitrage-bot

## Pinned environment

- Project commit: `fb98599c087a93aa03446553d55eb131507e6ba7`
- Test commit: `fb98599c087a93aa03446553d55eb131507e6ba7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 23.5 to 29 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 23.5 | 0 | 0 | [run](https://argusic.com/run/b8e039a3-3fbe-48e2-9bbf-e6c282ed4318) |
| 2 | pass with mocks | 72 | 30 | 29 | 3 | 0 | [run](https://argusic.com/run/a4574df9-1a90-4078-b692-82fcb85df0ec) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `solana-mev: 177 pre-existing compilation errors - missing types (AccountInfo, AccountMeta) and dependencies (spl_token, bincode, rand)`
- 3 min: `client-pool: dependency path ../program/programs/tmp does not exist, should be ../solana-program/programs/tmp; also has upstream indicatif build issue`
- 1 min: `Jupiter API quote-api.jup.ag DNS does not resolve in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
