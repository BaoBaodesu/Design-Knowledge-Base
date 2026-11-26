# 设计师知识库（Design Knowledge Base）

一套面向设计师与 AI 创作者的中文视觉设计参考库，整理了 **115 个精选设计网站**、**39 种设计风格档案**、**风格与受众匹配指南**、**30 套跨风格组合配方** 以及 **31 套 AI 视觉提示词模板**。

你可以直接拿它查灵感、定视觉方向、写 AI 出图提示词，也可以作为知识库接入 AI Agent，让它按规范完成选风、混搭、出图与验收。

---

## 你能在这里找到什么

### 1. 灵感网站与资源导航
- **[网站资源总表](01-sites.md)**：收录 100 个全球设计网站（覆盖大奖、动态、3D、UI、字体、配色等 9 大类）与 15 个常用中文/素材补充站，附用途说明与可访问状态。
- **[多维分类索引](04-taxonomy.md)**：按「用途」「领域」「风格」三个维度快速定位对应参考站。

### 2. 设计风格与受众决策
- **[设计风格与视觉特征](02-styles.md)**：29 种主流设计风格的配色、字体、版式、图形、质感、常见误区及对应参考站（区分“站点收录作品风格”与“站点自身界面风格”）。
- **[风格与目标受众对应表](03-style-audience.md)**：分析每种风格适合的人群、情绪印象、适用行业、使用边界与国内外平台差异。
- **[精选 10 大风格专题](05-top10-styles.md)**：提炼高频实用的 10 种核心风格（极简、瑞士网格、编辑风、新野兽派、Bento、玻璃拟态、深色科技、3D 黏土、Y2K、新中式/国潮），方便快速上手。
- **[风格分类体系与概念边界](09-style-taxonomy-and-relations.md)**：理清历史运动、平面体系、时代美学、界面风格与图像技法的区别（例如 Art Deco 与黑金、Y2K 与 Frutiger Aero、Glitch 与 Cyberpunk 的边界）。

### 3. 风格混搭与 AI 提示词
- **[混合风格组合方案](06-mixes.md)**：14 套经典双风格搭配，包含主次比例、组合逻辑、适用场景与避坑要点。
- **[扩展风格档案与视觉配方](10-visual-recipes.md)**：10 种扩展风格（构成主义、风格派、新艺术、装饰艺术、波普、Frutiger Aero、故障艺术、超现实拼贴、剪纸拼贴、野兽派平面）的馆藏级参考图，以及 16 套可直接套用的跨风格配方（R01–R16）。
- **[AI 视觉提示词模板](07-prompts.md)**：15 套主库中英文提示词模板（适配 Midjourney / Stable Diffusion 等），并索引 16 套扩展与高频风格的模块化提示词。

### 4. 给 AI Agent 使用的视觉设计系统
如果你希望 AI 辅助完成完整的设计方案，可以直接引导它阅读以下文档：
- **[Agent 使用说明](AGENTS.md)** & **[全库索引](llms.txt)**：任务路由、检索路径与输出规范。
- **[Agent 视觉设计工作流](08-agent-visual-design-system.md)**：从拆解需求、选风、组合到组装提示词的完整流程（含角色海报专用规则）。
- **[风格兼容矩阵与自主组合指南](12-style-compatibility-and-composition.md)**：9×9 类型兼容矩阵、视觉维度所有权规则与 6 步自主组合算法。
- **[视觉设计验收与评估标准](11-design-evaluation.md)**：10 项验收维度、评分权重与迭代优先级清单。

---

## 常见场景怎么用

| 你的需求 | 推荐查阅路径 |
|---|---|
| **快速找参考网站** | 先在 [04-taxonomy.md](04-taxonomy.md) 按领域/用途筛选，再到 [01-sites.md](01-sites.md) 看推荐用法 |
| **给项目定视觉风格** | 用 [05-top10-styles.md](05-top10-styles.md) 或 [02-styles.md](02-styles.md) 看特征，结合 [03-style-audience.md](03-style-audience.md) 判断受众匹配 |
| **想做跨风格混搭** | 参考 [06-mixes.md](06-mixes.md) 与 [10-visual-recipes.md](10-visual-recipes.md)，避坑与维度分配看 [12-style-compatibility-and-composition.md](12-style-compatibility-and-composition.md) |
| **写 AI 出图 / UI 提示词** | 直接套用 [07-prompts.md](07-prompts.md) 模板，或组合 [data/extended-prompts.json](data/extended-prompts.json) 的模块化词条 |
| **让 AI 自动化出方案** | 将 [AGENTS.md](AGENTS.md) 作为系统指令，让 Agent 检索 `data/` 下的 JSON 数据并按 [11-design-evaluation.md](11-design-evaluation.md) 自检 |

---

## 结构化数据（`data/`）

所有核心内容均同步沉淀为机器可读文件，方便脚本检索或接入工作流（字段说明见 [data/schema.md](data/schema.md)）：

- `data/kb.json`：全量基础数据（115 个网站、29 种风格、受众、精选 10 大风格、14 套组合、15 套提示词）。
- `data/style-relations.json`：10 种扩展风格完整档案、参考图、关系图谱及主库 29 种风格的类型映射。
- `data/visual-recipes.json`：16 套可复用视觉配方（R01–R16）。
- `data/compatibility-matrix.json`：9×9 类型兼容矩阵、维度所有权、交付物约束与 34 组风格对兼容规则。
- `data/extended-prompts.json`：16 种扩展与高频风格的模块化提示词（支持按版式/几何/配色/材质/光影拼装）。
- `data/sites.csv` / `data/styles.csv`：表格版网站与风格清单，可直接用 Excel 或 Notion 打开。
- `data/screenshots/`：网站首页截图拼图（编号对应网站 id）。

---

## 关于来源与更新

- **更新日期**：2026-11-26
- **参考来源**：优先整理自官方文档、博物馆/学术机构与专业设计社区，完整引用列表见 [sources.md](sources.md)。
- **链接核验**：全库 115 个网站均做过访问检查（已核验 110、部分核验 3、访问失败 2），明细见 [data/verification.tsv](data/verification.tsv)。
- **研究过程**：各轮整理与核对记录存档在 `notes/` 目录，供查阅背景与脉络。
