# JoySafeter

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jd-opensource/JoySafeter, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/joysafeter

## Pinned environment

- Project commit: `12234a11a9d96acef85577afb1fa5682169d6171`
- Test commit: `12234a11a9d96acef85577afb1fa5682169d6171`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 11 to 15.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 10 | 11 | 2 | 2 | [run](https://argusic.com/run/30f48319-c75c-406f-87e9-8338453f7c2a) |
| 2 | pass | 100 | 15 | 15.8 | 2 | 2 | [run](https://argusic.com/run/38ec8d04-d026-49e6-9a39-f7d48f08928f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_legacy_chat_frame_is_rejected_before_task_creation: test used deprecated 'type: chat' frame format not accepted by new protocol parser which only accepts 'chat.start'`
- 2 min: `test_run_chat_turn_emits_accepted_before_status: test mock for get_user_config returned 3 values (config, dict, model_info) but get_user_config now returns 2 values (config, dict)`

Attempt 2:

- 4 min: `Test test_legacy_chat_frame_is_rejected_before_task_creation: expected error message about "legacy metadata control fields" but the chat protocol was refactored so type "chat" is now unknown`
- 3 min: `Test test_run_chat_turn_emits_accepted_before_status: mock get_user_config returned 3-tuple but real function returns 2-tuple, causing ValueError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
