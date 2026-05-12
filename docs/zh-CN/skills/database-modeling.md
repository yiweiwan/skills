# database-modeling：数据库建模

## 文件位置

`.claude/skills/database-modeling/SKILL.md`

## 适用场景

仅作为通用数据库设计的总控/路由 skill 使用。schema 变更和回填使用 `database-migrations`，SQL 编写使用 `sql-querying`，慢查询和索引调优使用 `database-performance`。

## 能力重点

- 先查看现有 schema、迁移、ORM 模型和命名约定。
- 能使用更窄数据库 skill 时优先使用更窄 skill。
- 对长期有效的业务不变量使用数据库约束保护。
- 谨慎处理生产数据、非空字段、唯一约束和破坏性迁移。
- 根据真实查询模式添加索引。

## 示例提问

```text
请为多租户订单系统设计数据库表结构。
```

```text
帮我写一个安全的迁移，给用户表增加唯一邮箱约束。
```

```text
这个查询很慢，请分析索引和 SQL 写法。
```
