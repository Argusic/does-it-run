# tesseract

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tesseract-ocr/tesseract, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/tesseract

## Pinned environment

- Project commit: `76865fa087c15f5ea2f75f697993fc3b05eabaf2`
- Test commit: `76865fa087c15f5ea2f75f697993fc3b05eabaf2`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 25 to 38.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 34 | 34.9 | 6 | 6 | [run](https://argusic.com/run/e9ecb6fa-2423-434d-a664-1570645b33ae) |
| 2 | pass | 100 | 19 | 25 | 3 | 3 | [run](https://argusic.com/run/f6832bb4-4c65-4f06-a9b6-95be7108fbb1) |
| 3 | pass | 100 | 36 | 38.5 | 7 | 7 | [run](https://argusic.com/run/a5d5be93-7dd6-42f3-a67a-359d6a113f68) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `cmake not found on system`
- 10 min: `Missing all build dependencies (leptonica, pkg-config, libpng-dev, libtiff-dev, libjpeg-dev, libwebp-dev, zlib-dev, libgif-dev, libopenjp2-dev, libicu-dev, libzstd-dev, liblzma-dev, libdeflate-dev, libjbig-dev, libsharpyuv-dev)`
- 2 min: `pkg-config binary not available (only library packages)`
- 10 min: `Leptonica shared lib from .deb had broken transitive dependency chain (gif, openjp2, webpmux) and missing .so files`
- 5 min: `Linker errors for transitive static lib deps: libtiff requires libjbig, liblzma, libdeflate, libzstd, libLerc; libwebp requires libsharpyuv`
- 1 min: `No English language traineddata available`

Attempt 2:

- 5 min: `Leptonica library not found on system`
- 5 min: `Leptonica built without image I/O support (missing png/jpeg/tiff/zlib dev headers)`
- 4 min: `ICU dev headers missing for test build (BUILD_TESTS=ON requires icu-uc/icu-i18n)`

Attempt 3:

- 3 min: `Missing Leptonica and other -dev packages (no root apt install)`
- 2 min: `Static libarchive.a has unresolved zlib symbols at link time`
- 1 min: `libgif.so.7 not found at runtime linking`
- 2 min: `ICU headers not found (prefix=/usr hardcoded in .pc files)`
- 5 min: `Missing traineddata files for languages (eng, osd, heb, ara, chi_tra, jpn, vie, hin, kmr, script/Latin)`
- 5 min: `Missing langdata_lstm resources (radical-stroke.txt, hin/*, eng/*, font_properties, extendedhin/*)`
- `progress_test fails with progress reporting at exactly 99 failing Gt(99) assertion`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
