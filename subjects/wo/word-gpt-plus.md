# word-GPT-Plus

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Kuingsmile/word-GPT-Plus, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/word-gpt-plus

## Pinned environment

- Project commit: `065e25ebd2a0e50c409d33d8f0d5ff8f04712b5b`
- Test commit: `065e25ebd2a0e50c409d33d8f0d5ff8f04712b5b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31 to 31 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 31 | 4 | 4 | [run](https://argusic.com/run/847afb25-253e-411d-b5d8-5113a3658539) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node.js 18.19.1 failed the pinned-toolchain preinstall (project requires Node 24.21.0 / pnpm 12.11.2)`
- 5 min: `Backgrounded mock HTTP servers (nohup & subshell) were reaped by the exec harness after the parent shell exited, causing ECONNREFUSED on 127.0.0.1:11434`
- 2 min: `Harness-only bug: my in-memory checkpoint saver encoded bytes as JSON strings, breaking the real JsonPlusSerializer loadsTyped during agent putWrites`
- 1 min: `Temporary probe artifacts made 'pnpm format:check' report style issues`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
