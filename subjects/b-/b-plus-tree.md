# B-Plus-Tree

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/niteshkumartiwari/B-Plus-Tree, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/b-plus-tree

## Pinned environment

- Project commit: `100da060e6278f14864a45973a5055bd6c0adadf`
- Test commit: `100da060e6278f14864a45973a5055bd6c0adadf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.7 to 14.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 14.7 | 5 | 5 | [run](https://argusic.com/run/3018ce53-0caf-4f5d-91fb-e601d8ad4070) |
| 2 | pass | 100 | 4.5 | 14.7 | 3 | 3 | [run](https://argusic.com/run/815e732a-e96b-4103-a982-e4b774e8fdd7) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Makefile found in repo despite README claiming 'make' is the recommended build method`
- 3 min: `Double-free crash in bptree_demo insertionMethod() and basic_usage.cpp: fclose(filePtr) called after tree.insert() but tree also owns and closes the FILE*`
- 3 min: `Double-free crash in removal.cpp leaf node merge logic: FILE* handles transferred to sibling node but deleted node's destructor also closes them`
- 2 min: `CMake target missing for basic_usage example; CMakeLists parse error from duplicate install() line`
- 1 min: `test_suite.sh tries to run 'make' which fails when invoked via ctest from cmake binary dir (no Makefile there)`

Attempt 2:

- 1.5 min: `double-free crash in delete after insert: main.cpp fclose() on FILE* owned by tree`
- 2 min: `double-free crash during leaf-node merge in removeKey(): merged node destructor closed FILE* that had been transferred to surviving node`
- 0.5 min: `Makefile missing: test_suite.sh requires 'make' but repo only had CMakeLists.txt`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
