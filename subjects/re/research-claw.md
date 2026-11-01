# research-claw

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nanoAgentTeam/research-claw, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/research-claw

## Pinned environment

- Project commit: `ce3a4acd65d81f5f7681a90df0bf4abab288cc7d`
- Test commit: `ce3a4acd65d81f5f7681a90df0bf4abab288cc7d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.3 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.3 | 6 | 6 | [run](https://argusic.com/run/e29f7cd9-d998-40d1-88ae-c9016296fd12) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_default_max_tokens_is_capped_for_non_reasoning_models failed: max_tokens was None instead of 8192 (no default or clamping in OpenAIProvider)`
- `test_explicit_max_tokens_above_cap_is_clamped failed: max_tokens 20000 unclamped instead of 8192`
- 2 min: `test_custom_endpoint_prefers_protocol_over_model_name failed: LiteLLMProvider.__init__() got unexpected keyword argument 'provider_type'`
- `test_native_routing_prefers_protocol_over_model_name failed: same keyword argument issue`
- 1 min: `test_custom_endpoint_prefers_protocol_over_model_name: expected api_base url mismatch after base class normalization strips /v1`
- 1 min: `test_full_chain_with_parent_message failed: expected inbound_msg.channel 'feishu' but actual is 'im_feishu' (matching channel.name)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
