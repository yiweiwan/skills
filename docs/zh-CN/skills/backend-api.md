# backend-api：后端 API

## 文件位置

`.claude/skills/backend-api/SKILL.md`

## 适用场景

仅作为通用后端 API 的总控/路由 skill 使用。REST API 使用 `rest-api`，GraphQL 使用 `graphql-api`，认证和授权使用 `auth-access-control`。

## 能力重点

- 先理解框架、路由、验证层、错误模型和测试习惯。
- 能使用更窄 API 或权限 skill 时优先使用更窄 skill。
- 把传输层逻辑和业务逻辑分清楚。
- 在服务端边界进行输入校验和权限控制。
- 保持 API 状态码、错误结构、分页和过滤规则一致。

## 示例提问

```text
请帮我实现订单创建接口，包括参数校验、事务和错误处理。
```

```text
这个接口需要增加权限校验，请按现有后端模式修改。
```

```text
帮我为用户列表 API 增加分页和筛选。
```
