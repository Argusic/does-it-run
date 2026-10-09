# python-office

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CoderWanFeng/python-office, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/python-office

## Pinned environment

- Project commit: `dd6fe566f2125e3d09fb72e118d2840e74919034`
- Test commit: `dd6fe566f2125e3d09fb72e118d2840e74919034`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 26 to 26 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 26 | 12 | 12 | [run](https://argusic.com/run/246b8867-ff2b-4576-9f56-e0a07ff37a4b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PEP 668 externally-managed-environment blocked system pip install`
- 2 min: `pytest test_optional_imports failed: office.api.web._load_pospider raised ImportError (AttributeError on absent pospider.url) instead of ModuleNotFoundError`
- 2 min: `office.api.file had no search_by_content function while pofile's was a print-only stub and tests call it with content kwarg`
- 2 min: `office.api.pdf.add_text_watermark called popdf.add_watermark (no-arg stub) causing TypeError`
- 4 min: `missing test fixtures (tests/test_files) cause most file/excel/pdf/image test failures; the repo's own tests reference them but they are gitignored and not shipped`
- 1 min: `Windows-only deps (poppt/poword/PyOfficeRobot) not installed per setup.cfg on Linux; ppt/word/wechat tests fail ModuleNotFoundError by design`
- 1 min: `OCR (test_ocr) and downstream features need real Tencent SecretId/SecretKey`
- 1 min: `poimage add_watermark fails: bundled font msyh.ttc missing from installed poimage wheel`
- 1 min: `povideo.txt2mp3 needs eSpeak/espeak-ng system binary not present; video2mp3 works`
- 1 min: `poexcel fake2excel with column 'phone' errors: faker has no 'phone' provider`
- 2 min: `GUI Qt xcb plugin fails (libxcb-xinerama.so.0 missing; system packages cannot be installed, no root)`
- 1 min: `popdf.pdf2imgs TypeError: office/api/pdf.py passes keyword output_path which popdf's pdf2imgs does not accept (uses output_file)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
