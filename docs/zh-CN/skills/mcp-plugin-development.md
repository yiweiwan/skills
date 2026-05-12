# mcp-plugin-development：MCP 与插件开发

## 文件位置

`.claude/skills/mcp-plugin-development/SKILL.md`

## 适用场景

用于开发 MCP Server、Claude Code 插件、工具连接器、本地集成、插件 manifest、tool schema、resource template、权限、安装文档和 AI 工具扩展工作流。

## 能力重点

- 区分 MCP Server、Claude Code Plugin、connector 和本地工具集成。
- 让工具输入强类型、工具名称清晰、描述便于模型选择。
- 对有副作用的操作明确说明，并尽量设计为可重复执行。
- 输出结构化、紧凑、易于模型继续使用的数据。

## 示例提问

```text
请帮我设计一个 MCP Server，暴露查询内部知识库的工具。
```

```text
这个插件 manifest 需要补全权限和安装说明。
```

```text
请检查这个 tool schema 是否适合 Claude 调用。
```
