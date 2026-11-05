# mcp-agent

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lastmile-ai/mcp-agent, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-agent

## Pinned environment

- Project commit: `f62d849350816588b1c6294e7914bbe4d8b84072`
- Test commit: `f62d849350816588b1c6294e7914bbe4d8b84072`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 19.9 to 54.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass with mocks | 92 | 4.5 | 19.9 | 2 | 2 | [run](https://argusic.com/run/04323042-4061-4b1c-bf98-6d2e0e951956) |
| 2 | pass | 100 | 3 | 54.8 | 1 | 1 | [run](https://argusic.com/run/51f64b50-ca35-4cd5-a8f3-084298f9d469) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `Base class AugmentedLLM declared generate_stream as @abstractmethod but subclasses OpenAIAugmentedLLM, AzureAugmentedLLM, GoogleAugmentedLLM, Orchestrator, DeepOrchestrator, ParallelLLM, EvaluatorOptimizerLLM, Swarm, LMStudioAugmentedLLM, O`
- 2 min: `Bedrock streaming test expected usage tokens (input_tokens=100, output_tokens=50) but mock events did not include a metadata event with usage data, causing assertion failure`

Attempt 2:

- 25 min: `generate_stream abstract method not implemented in 8 source subclasses and 9 test mock classes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
