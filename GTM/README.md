# GTM — Go-to-Market Page

Awesome Company 的对外展示页（Go-to-Market）：向访客说明这个清单是什么、收录了多少、长什么样、怎么参与，并引导 Star 与贡献。

## 预览

```bash
# 在仓库根目录执行
python3 -m http.server 8123
# 打开 http://localhost:8123/GTM/
```

纯静态页面：无构建步骤、无 JavaScript、无外部依赖（仅 Google Fonts CDN）。

## 数据来源

页面中的统计数字（493 家公司 / 17 个分类 / 4 大板块 / 85 个地区）与示例条目均取自提交 `fbec59e` 时点的 `README.md`。收录数随贡献持续增长，以仓库 README 为准。

## 设计上下文

- `../PRODUCT.md` — 战略层：定位、用户、品牌个性（全面 · 严谨 · 可信）、反参照与设计原则
- 视觉系统：`styles.css` 顶部的自定义属性（OKLCH 色板、双字体栈、间距与层级）
