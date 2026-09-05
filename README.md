# quanttide-journal-of-strategy-management

量潮战略管理日志。

## 目录结构

日志按业务轴分目录，文件按日期命名：

- `default/` — 公司级/创始人视角，跨业务、跨职能的战略推演
- `qtdata/` — 量潮数据
- `qtclass/` — 量潮课堂
- `qtcloud/` — 量潮云
- `qtconsulting/` — 量潮咨询

## 条目元数据

每篇日志头部使用 YAML front-matter 声明战略层次与矩阵归属，正文保持自由记录风格：

```markdown
---
level: business
business: [qtclass]
functions: [org, growth]
---

正文……
```

### 字段定义

- `level`：战略层次，该条日志主要作用的层次，取值 `corporate`（公司战略）、`business`（业务战略）、`function`（职能战略）
- `business`：主属业务，正文主要在讲谁，单值原则，与所在目录一致；`default` 目录下为 `[corporate]`
- `functions`：涉及的职能，可多选

### 职能 taxonomy

- `org` — 组织管理
- `growth` — 增长管理
- `sales` — 销售管理
- `brand` — 品牌管理
- `media` — 新媒体运营
- `product` — 产品与技术

业务轴与职能轴构成战略矩阵：按行读是业务视角（进目录读日志），按列读是职能视角（按 `functions` 标签聚合），`level` 用于区分同一条目在公司、业务、职能三个层次上的不同作用面，共同为战略档案（profile）更新提供取材入口。
