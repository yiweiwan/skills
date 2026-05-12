---
name: excel-formulas
description: Use only when writing, explaining, debugging, or improving Excel or spreadsheet formulas, including lookup formulas, dynamic arrays, conditional logic, date formulas, financial formulas, named ranges, and formula errors.
---

# Excel Formulas

## Workflow

1. Identify spreadsheet app, locale, input columns, expected output, and edge cases.
2. Prefer readable formulas and helper columns over fragile mega-formulas.
3. Handle blanks, text numbers, dates, errors, and duplicates deliberately.
4. Explain formulas in plain language when requested.
5. Keep references stable for copy/fill behavior.

## Rules

- Use table references or named ranges when the workbook already uses them.
- Watch for comma versus semicolon separators by locale.
- Avoid volatile functions unless needed.

## Verification

- Test formula on normal, blank, duplicate, and error rows.
- Check totals and representative examples.
