# browser-extension：浏览器扩展

## 文件位置

`.claude/skills/browser-extension/SKILL.md`

## 适用场景

用于开发 Chrome、Edge、Firefox 或 Safari 浏览器扩展，包括 manifest、content script、background service worker、权限、storage、消息通信、popup UI、options 页面和 WebExtension 打包。

## 能力重点

- 明确 manifest 版本、目标浏览器、权限和打包方式。
- 区分 content script、background、popup、options 和共享逻辑。
- 使用最小权限，避免不必要的站点访问。
- 把网页 DOM、注入内容和扩展消息当作不可信输入处理。

## 示例提问

```text
请帮我实现一个 Chrome 扩展，在当前页面提取标题并显示到 popup。
```

```text
这个扩展的 content script 和 background 通信失败，请帮我排查。
```

```text
请检查 manifest 权限是否过大。
```
