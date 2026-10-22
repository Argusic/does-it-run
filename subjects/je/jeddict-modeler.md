# jeddict-modeler

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jeddict/jeddict-modeler, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/jeddict-modeler

## Pinned environment

- Project commit: `496fb1893c0bac111b737340187eb1f661eb732f`
- Test commit: `496fb1893c0bac111b737340187eb1f661eb732f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 33.8 to 51.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 21 | 33.8 | 4 | 4 | [run](https://argusic.com/run/d6052402-4107-4fc4-bf95-7ec024feab03) |
| 2 | fail | 50 | 13.2 | 51.2 | 5 | 5 | [run](https://argusic.com/run/5685593f-c39b-4ffb-87ff-4e6bd1b36ea1) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `JDK and Maven not installed in container`
- 2 min: `Missing modeler-lib dependency from sibling repo netbeans-modeler`
- 1 min: `nbm.build.dir default path (/work/jeddict-cluster) not writable`
- 1 min: `Compilation failure in ClassloaderTypeSolver.java - javaparser 3.25.1 moved TypeSolver interface and SymbolReference to com.github.javaparser.resolution package`

Attempt 2:

- 4.1 min: `No JDK or Maven available in container`
- 1.5 min: `HTTP repo bits.netbeans.org unreachable (connection refused on port 80)`
- 0.5 min: `Build failed: nbm plugin could not write to root-owned /work/jeddict-cluster`
- 2.1 min: `Build failed: jpa-spec compilation - TypeSolver/SymbolReference imports use old javaparser package`
- 5 min: `Tests fail: require NetBeans IDE 11.3+ platform runtime. Module system hangs on missing platform deps (commons-codec, commons-logging, gson, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
