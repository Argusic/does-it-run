# txtai

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/neuml/txtai, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/txtai

## Pinned environment

- Project commit: `483dbd3b3bd8d50bb7939bc75b11ef967543acdc`
- Test commit: `483dbd3b3bd8d50bb7939bc75b11ef967543acdc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 83 to 83 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 94.74 | 2 | 83 | 19 | 14 | [run](https://argusic.com/run/9e16211b-2cee-4b4c-a12b-caad2d4101db) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Externally-managed Python environment blocked system pip install`
- 1 min: `torchvision missing (transformers import error)`
- 2 min: `sentence-transformers not installed (testShortcuts ImportError)`
- 1 min: `scikit-learn/scipy missing (testwords ImportError)`
- 1 min: `grand-cypher/grand-graph missing (testShortcuts graph error)`
- 1 min: `apache-libcloud missing (testObjectStorage error)`
- 1 min: `smolagents missing (testagent ImportError)`
- 1 min: `gliner-py/sentencepiece missing (testGliner error)`
- 1 min: `chonkie/nltk/tika missing (testSentences, testChonkie errors)`
- 3 min: `docling/liteparse missing (testDocling, testLiteParse errors)`
- 1 min: `timm/imagehash missing (TimmBackbone error)`
- 1 min: `sounddevice/ttstokenizer/webrtcvad missing (TextToSpeech error)`
- 1 min: `fastapi-mcp missing (testmcp import error)`
- 1 min: `croniter/xmltodict missing (testScheduleWorkflow error)`
- `PEFT not installed (2 test errors)`
- `LiteRT and LiteLLM auth issues (2 test errors)`
- `Audio hardware not available (3 test errors)`
- `No Java for Tika and URL access restrictions (8 test errors)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
