# performance-optimization：性能优化

## 文件位置

`.claude/skills/performance-optimization/SKILL.md`

## 适用场景

仅作为性能问题的总控/路由 skill 使用。前端速度使用 `frontend-performance`，服务端速度使用 `backend-performance`，SQL 和数据库瓶颈使用 `database-performance`。

## 能力重点

- 先定义性能目标和用户可感知的问题。
- 先测量，再判断瓶颈在前端、后端还是数据库。
- 路由到更窄的性能 skill。
- 保持正确性，不用隐性可靠性代价换速度。

## 示例提问

```text
请分析这个页面首屏慢的原因并优化。
```

```text
这个接口 P95 延迟过高，请帮我定位瓶颈。
```

```text
请优化 CI 构建时间，但不要降低测试覆盖。
```
