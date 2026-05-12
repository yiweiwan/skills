# office-documents：办公文档

## 文件位置

`.claude/skills/office-documents/SKILL.md`

## 适用场景

仅作为办公文档的总控/路由 skill 使用。当任务可以明确归类时，优先使用更窄的 skill：Word 文档用 `word-document-editor`，PDF 用 `pdf-document-workflow`，报告用 `business-report-writing`，会议纪要用 `meeting-notes`，SOP 用 `sop-writing`，制度政策用 `policy-writing`，方案提案用 `proposal-writing`。

## 能力重点

- 先判断文档类型，再路由到更窄的 skill。
- 只在混合文档任务或初步分类时使用本 skill。
- 保留名称、日期、标题、编号和来源事实。
- 对法律、医疗、财务、HR、隐私和合规内容提示人工复核。

## 示例提问

```text
请把这份会议记录整理成正式纪要，包含决策和待办。
```

```text
帮我润色这份项目方案，让结构更清晰。
```

```text
请把这份 SOP 改成可执行的步骤清单。
```
