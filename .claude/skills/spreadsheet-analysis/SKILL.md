---
name: spreadsheet-analysis
description: Use as a router only for broad spreadsheet work. Prefer excel-formulas for formulas, csv-data-cleaning for CSV cleaning, and spreadsheet-dashboard for dashboards, KPI tables, pivots, and charts.
---

# Spreadsheet Analysis

## Workflow

1. Identify file format, sheets, columns, data types, row counts, formulas, and business meaning.
2. Route to `excel-formulas`, `csv-data-cleaning`, or `spreadsheet-dashboard` when applicable.
3. Preserve original data; work on a copy or add derived columns when editing files.
4. Validate totals before and after transformations.
5. Explain assumptions and data quality issues.

## Patterns

- KPI summary: definitions, period, filters, totals, averages, trends, exceptions.
- Reconciliation: expected total, actual total, variance, cause, owner.
- Forecast: inputs, assumptions, formula logic, scenarios, sensitivity.

## Verification

- Cross-check totals, row counts, unique keys, joins, and date ranges.
- Spot-check representative rows against the source.
