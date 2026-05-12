# observability-monitoring：可观测性与监控

## 文件位置

`.claude/skills/observability-monitoring/SKILL.md`

## 适用场景

仅作为可观测性任务的总控/路由 skill 使用。日志使用 `logging`，指标、Dashboard、健康检查、SLO 和告警使用 `metrics-alerting`，分布式链路追踪使用 `tracing`。

## 能力重点

- 明确服务边界、关键用户路径、失败模式和现有监控工具。
- 先判断需要日志、指标、告警、trace 还是组合。
- 能使用更窄 skill 时优先使用更窄 skill。
- 避免在日志和 telemetry 中泄露敏感信息。

## 示例提问

```text
请为这个支付接口补充结构化日志和关键指标。
```

```text
帮我设计一个 API 延迟和错误率 Dashboard。
```

```text
请为这个告警补一份排查 runbook。
```
