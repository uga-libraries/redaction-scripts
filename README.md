# redaction-scripts
Scripts for redacting content from digital files

## pdf-batch-redaction.py
**Batch PDF Redactor:**This script parses searchable (i.e. OCR-readable) PDFs to identify strings for redaction. It creates a "quad" around the specified area in the PDF and permanently deletes text within that area, replacing it with a black rectangle.

Using the optional argument "replace" will save a new redacted copy of the file and delete the unredacted original. If no argument is used, the script will automatically save a new file with "_redacted" in the file name alongside the original.

This script requires an installation of PyMuPDF in your Python environment: https://github.com/pymupdf/PyMuPDF#installation

Script usage: python path/to/script path/to/dir/for/redaction [replace]
