# ai-llm-integration：AI 与 LLM 集成

## 文件位置

`.claude/skills/ai-llm-integration/SKILL.md`

## 适用场景

仅作为 AI/LLM 功能的总控/路由 skill 使用。Prompt 使用 `prompt-engineering`，RAG 和检索使用 `rag-pipeline`，Agent 和工具调用使用 `agent-tool-calling`，评估使用 `llm-evaluation`。

## 能力重点

- 先判断任务属于 Prompt、检索、工具调用、评估还是集成胶水。
- 能使用更窄 skill 时优先使用更窄 skill。
- 控制成本、延迟、隐私和日志风险。
- 对模型输出设置稳定边界。

## 示例提问

```text
请设计一个 RAG 问答流程，包含检索、引用和失败兜底。
```

```text
帮我把这个聊天功能改成结构化输出。
```

```text
请为这个 Agent 设计一组最小评估用例。
```
