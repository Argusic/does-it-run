# Upsonic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Upsonic/Upsonic, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/upsonic

## Pinned environment

- Project commit: `101f0313b0ddb96cd4078354879b2ff57005db29`
- Test commit: `101f0313b0ddb96cd4078354879b2ff57005db29`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 23.4 to 43.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 43 | 0 | 0 | [run](https://argusic.com/run/c8e548e4-6440-461c-bf73-d25adb032dde) |
| 1 | pass | 100 | 22 | 23.4 | 3 | 3 | [run](https://argusic.com/run/31f501a8-7551-4381-8e8d-85f05ce26cda) |
| 2 | timeout | none | 22 | 43.6 | 2 | 0 | [run](https://argusic.com/run/424cfefc-0494-4caf-810a-bf3e34822fde) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing beautifulsoup4 and lxml for HTMLChunker`
- 15 min: `Missing optional dependencies for loaders (aiofiles, jq, pypdf, pymupdf, python-docx, etc), vectordb (chromadb, qdrant-client, etc), embeddings (boto3, google-genai, etc)`
- 2 min: `Integration tests failed: test_ralph_real_world.py used non-existent method remove_from_fix_plan (should be remove_pending_item) and action="remove" (should be action="delete")`

Attempt 2:

- 8 min: `Milvus integration tests fail in milvus-lite embedded mode because gRPC AllocTimestamp is not implemented in milvus-lite`
- 5 min: `HuggingFace embedding tests fail because PyTorch is not installed (transformers import chain requires torch)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
