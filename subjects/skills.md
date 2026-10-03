# skills

**Verdict: runs.** Argusic Score 92.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-act/skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/skills

## Pinned environment

- Project commit: `11c057b03f92101642cadc9f840564574120d184`
- Test commits: `f004524de788065fcfbbdb8b07ee69493c6ec190`, `11c057b03f92101642cadc9f840564574120d184`, `a25c7851213d0d6a29422409fb1118f49c9f90af`, `eb07be67e6d924b958445f706f5ac386243df6b4`, `23d0dac5f83f268166a17f0bc7dc6c73dc348a33`, `a10738f076bedf4683573f896d8dc814f13d3b04`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible, real run
- Valid runs: 7; wall time 2.2 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 9.5 | 5 | 5 | [run](https://argusic.com/run/8405f33c-bf9c-4bed-a684-686a47b58e16) |
| 1 | fail | 80 | 12 | 7.9 | 3 | 3 | [run](https://argusic.com/run/65424f1f-7048-4b53-b2ae-77b93f8be507) |
| 1 | pass with mocks | 92 | 2 | 6.8 | 0 | 0 | [run](https://argusic.com/run/d04eb4bb-b8ee-4469-9583-4af239792d2c) |
| 1 | pass | 100 | 15.2 | 2.2 | 1 | 1 | [run](https://argusic.com/run/b9f95b51-1283-474b-b40f-7602c5b00066) |
| 1 | pass with mocks | 92 | 2.1 | 7.8 | 4 | 4 | [run](https://argusic.com/run/18801799-dce4-4c4c-9b72-e2940b119c91) |
| 1 | pass | 100 | 13 | 14 | 4 | 4 | [run](https://argusic.com/run/d29fc2ca-924b-4c33-aaa7-e1b7f9112c73) |
| 2 | pass | 90 | 6 | 5.3 | 6 | 3 | [run](https://argusic.com/run/0bd740fb-2706-4a9c-970c-daf389a749d2) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npx skills add google/skills requires Node >=22.20.0, container has v18.19.1`
- 2 min: `assemble_widget_proto_test.py: absltest.TestCase.create_tempdir() fails with unparsed flags`
- 2 min: `fetch_terraform_template_test.py: absl flags accessed before parsing`
- 2 min: `list_terraform_templates.py: DuplicateFlagError when imported alongside sibling module`

Attempt 1:

- 1 min: `pip3 install blocked by externally-managed-environment (PEP 668)`
- 1 min: `Skill handshake version mismatch blocked browser commands on first run`
- 2 min: `Chrome/Chromium not found for chrome-direct browser sessions`

Attempt 1:

- 14.5 min: `npm run check failed because AGENT_NATIVE_FRAMEWORK_PATH was not set and ../agent-native/framework did not exist`

Attempt 1:

- 0.5 min: `pnpm not available globally (no root); used npx pnpm instead`
- 1 min: `Node v18 < v22 requirement; harness runner works but vitest unit tests fail`
- `rolldown native binary missing: rolldown-binding.linux-x64-gnu.node not in pnpm store; vitest cannot start`

Attempt 1:

- 10 min: `dangerous-patterns.txt missing - the guard script (~/.agents/hooks/deny-dangerous.sh) references ~/.agents/hooks/dangerous-patterns.txt but the file did not exist`
- 1 min: `~/.agents/ directory did not exist - the guard scripts reference ~/.agents/hooks/ but the directory was not present`

Attempt 2:

- 0.5 min: `uv tool not found after pip install (PATH issue)`
- 0.5 min: `pip3 install uv blocked by externally-managed-environment`
- 2 min: `Skill version incompatible block: CLI refused all commands`
- 2 min: `auth set rejects API keys with server-side Invalid authorization`
- 2 min: `stealth-extract requires a BrowserAct API key (server-side validated, cannot mock)`
- 1 min: `chrome-direct type requires local Chrome installation (not available in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
