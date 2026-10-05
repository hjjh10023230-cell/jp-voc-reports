# JP VOC Reports

JP 市场 VOC 报告中心，统一归档 THEME、EVENT 与 VOC 用户问题报告。

## 对外链接

- 报告中心：首页 `https://hjjh10023230-cell.github.io/jp-voc-reports/`
- 最新一期：`https://hjjh10023230-cell.github.io/jp-voc-reports/latest.html`
- 历史报告：从首页进入，或使用各报告独立目录链接

## 目录规则

每份报告独立放在以下路径：

```text
reports/<年份>/<开始日期>_to_<结束日期>/index.html
```

示例：

```text
reports/2026/2026-09-28_to_2026-10-04/index.html
```

## 新增一期报告

1. 创建新的日期目录并放入 `index.html`。
2. 在 `reports.json` 最前面加入报告元数据。
3. 在站点首页加入报告卡片。
4. 把 `latest.html` 指向新报告。
5. 提交并推送到 `main`，GitHub Pages 会自动发布。

如果由 Claude Code 维护，只需要说：**“把这份 JP VOC 报告发布到报告中心”**。

## 安全要求

这是公开 GitHub 仓库和公开网页。发布前必须去除 UID、账户号、姓名、电话、邮箱、原始私聊记录和其他敏感信息。`robots=noindex` 仅表达不希望搜索引擎索引，不能替代访问控制。
