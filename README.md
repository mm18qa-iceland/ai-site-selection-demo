# AI 选址评估模型 · 作品演示（脱敏版）

"业务专家 + AI 编程助手"结对开发的连锁门店选址决策工具，纯前端零依赖（HTML + ECharts + OpenStreetMap）。

## 在线查看

- **作品说明（先看这个）**：https://mm18qa-iceland.github.io/ai-site-selection-demo/
- **模型演示入口**：https://mm18qa-iceland.github.io/ai-site-selection-demo/demo/overview.html
  - 城市准入评估：`demo/index.html`
  - 标准店点位评估：`demo/evaluation.html`

## 模型是什么

一道双层漏斗、三层串行闸口：

1. **城市准入**：K₁ 城市消费力 × K₂ 市场成熟度（艾灸养生 POI 密度钟形函数），乘积对照阈值表给三档结论；
2. **点位闸口**：9 项位置量特征（OSM 客观抓取）→ 商圈类型决策树 → 五项工程/合规红线一票否决；
3. **评分与财务**：对照在营门店基线的百分位评分（100 分制）→ 简版财务测算 + 行业基准校验 + 合规前置过滤。

品牌名已脱敏为"XX品牌"；演示数据为内置确定性示例值。

## 本地运行

无需安装，浏览器直接打开 `demo/overview.html`（两个评估页通过页面按钮互相跳转）。
