# Autonomous-Company

**Verdict: runs.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MaxMiksa/Autonomous-Company, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/autonomous-company

## Pinned environment

- Project commit: `c7c60dbd40d2d122adaad107f378420f8d614d7a`
- Test commit: `c7c60dbd40d2d122adaad107f378420f8d614d7a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.3 to 18.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 88 | 50 | 18.3 | 5 | 2 | [run](https://argusic.com/run/fcd0b7b2-229c-45e1-84a7-052d8bef970f) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `test_ui_messages.OperatorMessageTests.test_native_bash_nounset_handles_messages_with_and_without_parameters fails deterministically: ui_message language.saved en emits the zh-CN template while the container locale is C.UTF-8 (no zh-* env),`
- 10 min: `Browser and Node-20 suites cannot run: container has only Node 18.19.1 (playwright requires >=20, refused to download Chromium) and no other Node binary or root to install one.`
- 5 min: `Tailwind oxide native binding missing in dashboard/ui build (npm 9 + Node 18 optional-dependency bug, @tailwindcss/oxide-linux-x64-gnu absent); only reproducible on the CI-pinned Node 22 which is unavailable.`
- 5 min: `examples/scopefence test fails 1/8: 'crypto is not defined' in scopefence-core.js makeReceipt/randomUUID on Node 18 (browser-only global); unrelated to the framework runtime.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
