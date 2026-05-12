# Claude Code 通用 Skills

[![Skills](https://img.shields.io/badge/Claude%20Code-Skills-111827)](#skills-矩阵)
[![Language](https://img.shields.io/badge/docs-中文-blue)](docs/zh-CN/使用指南.md)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

一套面向日常开发、AI 应用、工程交付和办公协作的 Claude Code 通用 skills。

这些 skills 遵循 Claude skills 的基本形态：每个 skill 都是一个独立文件夹，核心文件是 `SKILL.md`，通过 frontmatter 中的 `name` 和 `description` 触发使用。

当前包含 73 个 skills。新版结构遵循“窄 skill 优先”：PPT 就只管 PPT，邮件就只管邮件，SQL 就只管 SQL；少数宽泛 skill 只作为总控/路由使用。

## 为什么用这套 Skills

- 覆盖面广：前端、后端、全栈、移动端、数据、AI、DevOps、GitHub、办公文档。
- 能力边界清楚：单一能力单独成 skill，减少触发冲突。
- 可直接使用：复制 `.claude/skills` 到项目即可。
- 结构清晰：每个 skill 只保留可执行流程、检查点和验证方式。
- 适合开源：包含 README、中文指南、分类目录、贡献说明和许可证。

## 快速开始

### 项目级安装

将 `.claude` 目录复制到你的项目根目录：

```powershell
Copy-Item -Recurse .\.claude C:\path\to\your-project\
```

安装后结构应类似：

```text
your-project/
  .claude/
    skills/
      frontend-design/
        SKILL.md
      backend-api/
        SKILL.md
```

### 用户级安装

如果你的 Claude Code 版本支持用户级 skills，可复制到用户目录：

```powershell
New-Item -ItemType Directory -Force $HOME\.claude\skills
Copy-Item -Recurse .\.claude\skills\* $HOME\.claude\skills\
```

## 使用示例

自然描述任务即可：

```text
帮我审查这个 PR，重点看数据一致性、安全和遗漏测试。
```

```text
请实现这个订单接口，包含参数校验、事务、错误处理和测试。
```

```text
把这些竞品资料整理成一页管理层决策简报。
```

也可以显式指定：

```text
请使用 frontend-design skill 优化这个后台页面。
```

```text
请使用 ai-llm-integration skill 设计这个 RAG 问答流程。
```

## Skills 矩阵

| 分类 | Skills |
| --- | --- |
| AI 与 Agent | `prompt-engineering`, `rag-pipeline`, `agent-tool-calling`, `llm-evaluation`, `ai-llm-integration`, `mcp-plugin-development` |
| 前端与客户端 | `frontend-design`, `react-frontend`, `vue-frontend`, `nextjs-frontend`, `frontend-performance`, `frontend-implementation`, `mobile-app-development`, `browser-extension` |
| 后端与数据 | `rest-api`, `graphql-api`, `auth-access-control`, `backend-api`, `database-migrations`, `sql-querying`, `database-performance`, `database-modeling`, `data-engineering`, `fullstack-integration` |
| 工程质量 | `testing-quality`, `debugging-troubleshooting`, `code-review`, `code-refactor`, `code-review-refactor`, `security-hardening` |
| 性能与可观测性 | `frontend-performance`, `backend-performance`, `database-performance`, `performance-optimization`, `logging`, `metrics-alerting`, `tracing`, `observability-monitoring` |
| 工程协作与交付 | `git-branch-commit`, `github-pr-issues`, `release-notes`, `git-github-workflow`, `monorepo-maintenance`, `devops-deployment`, `automation-scripting` |
| 产品、项目与研究 | `product-requirements`, `project-planning`, `web-research`, `competitor-analysis`, `document-summarization`, `literature-review`, `research-synthesis` |
| 文档、PPT、邮件与表格 | `readme-writing`, `api-documentation`, `runbook-writing`, `architecture-docs`, `word-document-editor`, `pdf-document-workflow`, `business-report-writing`, `meeting-notes`, `sop-writing`, `policy-writing`, `proposal-writing`, `presentation-builder`, `pitch-deck-builder`, `speaker-notes`, `email-drafting`, `stakeholder-update`, `excel-formulas`, `csv-data-cleaning`, `spreadsheet-dashboard`, `technical-writing`, `office-documents`, `email-communication`, `spreadsheet-analysis` |

## 仓库结构

```text
.claude/skills/                  # Claude Code 实际读取的 skills
docs/zh-CN/                      # 中文使用文档
README.md                        # 项目首页
skills-directory.md              # 总目录
CONTRIBUTING.md                  # 贡献指南
LICENSE                          # MIT License
```

## 文档

- [中文使用指南](docs/zh-CN/使用指南.md)
- [Skills 总目录](skills-directory.md)
- [各 Skill 中文说明](docs/zh-CN/skills/README.md)

## 设计原则

- `description` 写清楚触发场景。
- `SKILL.md` 正文只写流程、约束、检查点和验证方式。
- 一个 skill 只解决一类任务，避免变成百科全书。
- 宽泛 skill 只做路由，明确任务后使用更窄 skill。
- 优先通用、可复用、跨技术栈的工作流。
- 对高风险任务强调测试、验证、权限、安全和回滚。

## 参考资料

- [Claude Code Skills 官方文档](https://code.claude.com/docs/en/skills)
- [Anthropic skills 公共仓库](https://github.com/anthropics/skills)

## 贡献

欢迎提交新的 skill 或改进现有 skill。请参考 [CONTRIBUTING.md](CONTRIBUTING.md)。

## 许可

MIT License。详见 [LICENSE](LICENSE)。
