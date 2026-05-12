# monorepo-maintenance：Monorepo 维护

## 文件位置

`.claude/skills/monorepo-maintenance/SKILL.md`

## 适用场景

用于 Monorepo、workspace、包边界、共享库、依赖图、Nx、Turborepo、pnpm/yarn/npm workspaces、Bazel、构建缓存、版本管理和跨包重构。

## 能力重点

- 明确 workspace 管理器、包依赖图、构建系统和影响范围。
- 找到最小受影响包集合。
- 维护公共包 API 的兼容性。
- 同步更新共享类型、生成物和 package exports。

## 示例提问

```text
请把这个工具函数抽到 shared 包，并更新引用。
```

```text
帮我分析这个 monorepo 里哪些包会受改动影响。
```

```text
请修复 workspace 依赖版本不一致的问题。
```
