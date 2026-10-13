# JP KA VOC Weekly Reports

JP KA VOC周报中心，按周归档内部客户反馈、用户投资关注、外部公开舆情与风险／机会信号。

## 在线入口

- 报告中心：`https://hjjh10023230-cell.github.io/jp-voc-reports/`
- 最新周报：`https://hjjh10023230-cell.github.io/jp-voc-reports/latest-weekly.html`
- 固定最新链接：`https://hjjh10023230-cell.github.io/jp-voc-reports/latest.html`
- 历史周报：从报告中心进入，或访问对应周期目录

## 目录规则

```text
reports/<年份>/<开始日期>_to_<结束日期>/index.html
```

## 新增一期周报

1. 运行六类人群周数据提取，输出必须放在仓库外：

   ```powershell
   node scripts/fetch_ka_voc_week.js --start YYYY-MM-DD --end YYYY-MM-DD --output <仓库外JSON>
   ```

2. 核对KA整体及五类细分人群；细分人群无反馈时只写“暂无新增反馈”。
3. 创建周期目录并生成 `index.html`。
4. 更新 `reports.json`、首页、`latest.html`和`latest-weekly.html`。
5. 只展示信号、趋势与最简方向提示，不输出完整运营方案。
6. 发布前检查数据口径、来源去重、低样本表述和敏感信息。
7. 提交并推送到 `main`，GitHub Pages自动更新。

## 固定周报结构

1. 周度总结与关键指标；
2. 内部VOC：热门问题、板块／事件、热门个股；
3. 外部舆情：主题、个股、市场关注问题；
4. 风险／机会发现；
5. 最多3条方向提示；
6. 折叠的数据来源与口径。

全量反馈进入分析，但正文只展示重要信号。外部舆情按独立编辑来源去重；没有稳定数据时不展示虚假精确热度。

## 安全要求

这是公开GitHub仓库和公开网页。发布前必须去除UID、账户号、姓名、电话、邮箱、内部链接、原始私聊记录和其他敏感信息。`robots=noindex`不能替代访问控制。
