# data-engineering：数据工程

## 文件位置

`.claude/skills/data-engineering/SKILL.md`

## 适用场景

用于数据管道、ETL/ELT、批处理、流处理、数据验证、数仓、lakehouse、dbt、Airflow、Dagster、数据摄取、转换、回填和数据质量检查。

## 能力重点

- 明确来源、目标、schema、刷新频率、数据量和责任边界。
- 设计可重跑、可回填、可验证的数据流程。
- 检查行数、唯一性、空值、枚举值、引用完整性和时间窗口。
- 处理迟到数据、重复数据、schema 漂移和部分失败。

## 示例提问

```text
请设计一个订单数据从业务库同步到数仓的 ETL 流程。
```

```text
帮我给这个 dbt 模型补数据质量测试。
```

```text
请为这次历史数据回填写执行和校验步骤。
```
