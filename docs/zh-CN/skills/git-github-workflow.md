# git-github-workflow：Git 与 GitHub 工作流

## 文件位置

`.claude/skills/git-github-workflow/SKILL.md`

## 适用场景

仅作为 Git/GitHub 工作流的总控/路由 skill 使用。本地分支、提交和冲突使用 `git-branch-commit`，GitHub PR 和 Issue 使用 `github-pr-issues`，Release Notes 和 Changelog 使用 `release-notes`。

## 能力重点

- 先判断任务是本地 Git、GitHub 协作、发布说明还是仓库治理。
- 能使用更窄 skill 时优先使用更窄 skill。
- 不覆盖用户已有改动。
- 仓库协作文案保持清楚、可审查。

## 示例提问

```text
请帮我整理这次改动的 PR 描述。
```

```text
请解决这个 merge conflict，保留双方有效逻辑。
```

```text
帮我生成一版 release notes。
```
