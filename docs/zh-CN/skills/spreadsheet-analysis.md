# spreadsheet-analysis：表格分析

## 文件位置

`.claude/skills/spreadsheet-analysis/SKILL.md`

## 适用场景

仅作为通用表格任务的总控/路由 skill 使用。公式使用 `excel-formulas`，CSV 清洗使用 `csv-data-cleaning`，仪表盘、KPI、透视表和图表使用 `spreadsheet-dashboard`。

## 能力重点

- 先识别文件格式、sheet、列、数据类型、行数、公式和业务含义。
- 能使用更窄表格 skill 时优先使用更窄 skill。
- 保留原始数据，编辑时使用副本或派生列。
- 处理表头、类型、空值、重复、日期、货币、编码和异常值。
- 转换前后校验总数和关键指标。

## 示例提问

```text
请清洗这个 CSV，并输出各渠道销售额汇总。
```

```text
帮我设计一个项目进度跟踪表。
```

```text
请检查这个 Excel 公式为什么结果不对。
```
