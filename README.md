# CI Native Artifact Fixtures

This repository provides a stable matrix of files for testing Harness CI native artifact upload, listing, preview, relative-link navigation, download, and cross-stage reuse.

## Fixture coverage

- Root-level, extensionless, empty, hidden, and binary files
- HTML reports with relative links and nested folders
- JSON, XML, YAML, CSV, LOG, TXT, SVG, PNG, and PDF files
- Paths and filenames containing spaces
- A complete multi-page JaCoCo HTML coverage report

The JaCoCo report under `reports/jacoco/` is the `org.jacoco.core` coverage sample published at [`jacoco.org/jacoco/trunk/coverage/org.jacoco.core/`](https://www.jacoco.org/jacoco/trunk/coverage/org.jacoco.core/). Its original directory layout is preserved for preview, styling, and relative-link navigation testing.
