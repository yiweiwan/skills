# Skills Directory

本仓库提供 73 个 Claude Code skills。新版结构遵循“窄 skill 优先”：单一能力单独成 skill，宽泛 skill 只作为总控/路由使用。

Claude Code 可识别的 skill 文件位于 `.claude/skills/<skill-name>/SKILL.md`。

## 分类

| 分类 | Skills |
| --- | --- |
| AI 与 Agent | `prompt-engineering`, `rag-pipeline`, `agent-tool-calling`, `llm-evaluation`, `ai-llm-integration`, `mcp-plugin-development` |
| 前端与客户端 | `frontend-design`, `react-frontend`, `vue-frontend`, `nextjs-frontend`, `frontend-performance`, `frontend-implementation`, `mobile-app-development`, `browser-extension` |
| 后端、API 与权限 | `rest-api`, `graphql-api`, `auth-access-control`, `backend-performance`, `backend-api`, `fullstack-integration` |
| 数据库与数据 | `database-migrations`, `sql-querying`, `database-performance`, `database-modeling`, `data-engineering` |
| 测试、调试、安全与质量 | `testing-quality`, `debugging-troubleshooting`, `code-review`, `code-refactor`, `code-review-refactor`, `security-hardening` |
| 性能与可观测性 | `frontend-performance`, `backend-performance`, `database-performance`, `performance-optimization`, `logging`, `metrics-alerting`, `tracing`, `observability-monitoring` |
| GitHub、交付与自动化 | `git-branch-commit`, `github-pr-issues`, `release-notes`, `git-github-workflow`, `devops-deployment`, `monorepo-maintenance`, `automation-scripting` |
| 产品、项目与研究 | `product-requirements`, `project-planning`, `web-research`, `competitor-analysis`, `document-summarization`, `literature-review`, `research-synthesis` |
| 文档、PPT、邮件与表格 | `readme-writing`, `api-documentation`, `runbook-writing`, `architecture-docs`, `word-document-editor`, `pdf-document-workflow`, `business-report-writing`, `meeting-notes`, `sop-writing`, `policy-writing`, `proposal-writing`, `presentation-builder`, `pitch-deck-builder`, `speaker-notes`, `email-drafting`, `stakeholder-update`, `excel-formulas`, `csv-data-cleaning`, `spreadsheet-dashboard`, `office-documents`, `email-communication`, `spreadsheet-analysis`, `technical-writing` |

## 总控/路由 Skills

这些 skill 用于任务范围不清时做初步判断，明确后应优先使用更窄 skill：

- `ai-llm-integration`
- `frontend-implementation`
- `backend-api`
- `database-modeling`
- `code-review-refactor`
- `performance-optimization`
- `observability-monitoring`
- `git-github-workflow`
- `office-documents`
- `email-communication`
- `spreadsheet-analysis`
- `research-synthesis`
- `technical-writing`

## 中文文档

- [中文使用指南](docs/zh-CN/使用指南.md)
- [各 Skill 中文说明](docs/zh-CN/skills/README.md)
