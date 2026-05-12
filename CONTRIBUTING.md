# Contributing

欢迎贡献新的 Claude Code skills 或改进现有内容。

## 新增 Skill

1. 在 `.claude/skills/<skill-name>/SKILL.md` 创建 skill。
2. `skill-name` 使用小写字母、数字和连字符。
3. `SKILL.md` 必须包含 frontmatter：

```markdown
---
name: your-skill-name
description: Clear description of what this skill does and when to use it.
---
```

4. 正文保持简洁，优先写工作流、约束、检查点和验证方式。
5. 在 `docs/zh-CN/skills/<skill-name>.md` 增加中文说明。
6. 更新 `README.md`、`skills-directory.md`、`docs/zh-CN/使用指南.md` 和 `docs/zh-CN/skills/README.md`。

## 修改 Skill

- 保持变更聚焦，不把多个不相关主题塞进同一个 skill。
- 如果一个 skill 变得过宽，优先拆分。
- 不要在 `SKILL.md` 中加入过长背景知识。
- 高风险流程要包含验证、回滚或人工复核提示。

## 发布前检查

```powershell
Get-ChildItem .\.claude\skills -Directory | ForEach-Object {
  python <path-to-quick_validate.py> $_.FullName
}
```

## 隐私检查

发布前建议检查以下内容不要进入仓库：

- 个人草稿、Office 文档、PDF、压缩包和数据库文件。
- `.env`、证书、私钥、token、API key、cookie 和凭据文件。
- 本机绝对路径、用户名、手机号、邮箱、身份证号和内部系统地址。
- 真实客户、公司、项目、合同或财务数据。

可用以下命令做基础扫描：

```powershell
rg -n --hidden -S "C:\\Users|api[_-]?key|secret|token|password|private[_-]?key|BEGIN .*PRIVATE KEY|[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}" .
```

如果你不在本机环境，可以至少手动检查：

- 每个目录都有 `SKILL.md`
- frontmatter 只有 `name` 和 `description`
- `name` 与目录名一致
- 中文文档链接可打开
