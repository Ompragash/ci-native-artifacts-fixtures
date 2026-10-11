# CI Native Artifact Fixtures

This repository provides a stable matrix of files for testing Harness CI native artifact upload, listing, preview, relative-link navigation, download, and cross-stage reuse.

## Fixture coverage

- Root-level, extensionless, empty, hidden, and binary files
- HTML reports with relative links and nested folders
- JSON, XML, YAML, CSV, LOG, TXT, SVG, PNG, and PDF files
- Paths and filenames containing spaces
- A complete multi-page JaCoCo HTML coverage report

The JaCoCo report is the `org.jacoco.core` coverage sample published at [`jacoco.org/jacoco/trunk/coverage/org.jacoco.core/`](https://www.jacoco.org/jacoco/trunk/coverage/org.jacoco.core/).

- `reference/jacoco-official/` preserves the downloaded report exactly.
- `reports/jacoco/` is the upload fixture. HAR does not currently accept `$` in artifact paths, so the 49 inner-class filenames use `~` and their internal links are rewritten accordingly. The report content, layout, assets, and navigation are otherwise unchanged.
