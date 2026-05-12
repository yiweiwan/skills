---
name: csv-data-cleaning
description: Use only when cleaning, normalizing, validating, deduplicating, transforming, merging, or exporting CSV and flat tabular files, including encodings, delimiters, headers, data types, missing values, and row-count checks.
---

# CSV Data Cleaning

## Workflow

1. Identify delimiter, encoding, headers, row count, data types, and target output.
2. Preserve the original file and write cleaned output separately when editing files.
3. Normalize headers, dates, numbers, categories, whitespace, and missing values.
4. Deduplicate only with an explicit key or rule.
5. Validate row counts and key aggregates before and after.

## Rules

- Use CSV parsers instead of string splitting.
- Watch for quoted delimiters, newlines inside fields, and BOM markers.
- Keep transformation assumptions visible.

## Verification

- Compare input and output row counts.
- Spot-check representative rows and edge cases.
