# 设计师知识库 v1（design-kb）

一个中文设计参考知识库：100 个设计网站的分类资源库、29 种设计风格的视觉特征、风格与受众的对应关系、精选 10 大风格专题、混合风格组合方案，以及 AI 视觉提示词模板。每条信息都保留来源和核验状态，既方便人查阅，也方便 AI Agent 检索（见 [AGENTS.md](AGENTS.md)、[llms.txt](llms.txt)）。

- **更新日期**：2026-11-15（Asia/Shanghai）
- **初始学习资料**：Eian（[@EianLu](https://x.com/EianLu)）的 X 长文《100 个提升审美的设计网站大赏》：https://x.com/EianLu/status/2121219503988113557
- **范围**：原文正好列了 100 个网站（9 类），全部收录；另有 15 个站点标注为「文章之外补充」（中文站和常用素材站），不计入 100。
- **研究规范**：不搜索、不打开、不引用 CSDN（csdn.net）。无法确认的信息写「未核验」，没有数据支撑的受众判断写「推测」。

## 目录结构

```
design-kb-repo/
├── README.md               # 本文件（给人看）
├── AGENTS.md               # 给 AI Agent 的使用说明
├── llms.txt                # llmstxt.org 格式的索引
├── 01-sites.md             # 表一 网站资源总表（100 + 扩展 15，逐站核验）
├── 02-styles.md            # 表二 设计风格分类表 + 29 种风格详解 + 网站×风格映射
├── 03-style-audience.md    # 风格与目标受众对应表（含依据类型）
├── 04-taxonomy.md          # 多维分类：用途 / 领域 / 风格索引
├── 05-top10-styles.md      # 精选 10 大风格专题
├── 06-mixes.md             # 14 个混合风格组合方案
├── 07-prompts.md           # 15 种风格的中英文 AI 提示词模板
├── sources.md              # 引用来源与访问状态
├── notes/                  # 五轮研究笔记（round1–round5）
└── data/
    ├── kb.json             # 全量结构化数据（网站、风格、受众、精选、组合、提示词）
    ├── schema.md           # kb.json 与 CSV 字段说明
    ├── sites.csv           # 网站表（115 行）
    ├── styles.csv          # 风格表（29 行）
    ├── verification.tsv    # 逐站核验记录
    ├── article-100-list.json  # 原文 100 个网站清单（名称、链接、原文摘要）
    └── screenshots/        # 首页截图拼图（编号对应网站 id，2026-11-15）
```

## 核验图例

| 标记 | 含义 |
|---|---|
| ✅ 已核验 | 本次实际访问成功（curl 2xx 且标题正确，或 WebFetch 取得正文，或无头浏览器渲染出页面） |
| 🟡 部分核验 | 站点有响应，但只拿到部分内容（安全校验、间歇性错误） |
| ❌ 访问失败 | 多种方法都失败，已写明原因 |
| ⚪ 未核验 | 信息只来自原文或二手描述，未独立确认（如原文里的条目数量） |
| 🔮 推测 | 没有数据支撑的编者判断（主要是受众偏好、组合比例） |

受众判断的依据另分三级：**有据**、**部分有据**、**推测**（见 03-style-audience.md）。

## 核验概况（2026-11-15）

- 原文 100 个：已核验 97，部分核验 2（ASC：Cloudflare 520 间歇报错；Shadertoy：安全校验），访问失败 1（Realtime Colors：HTTP 402，部署已暂停）。
- 扩展 15 个：已核验 13，部分核验 1（Unsplash：反爬校验），访问失败 1（UI中国：TLS 连接被重置，疑为检测环境网络问题）。
- 检查方法：curl → WebFetch → 无头 Chrome 截图。网站会变，引用前建议复查。

## Agent 可调用视觉设计系统（v2 扩展）

在原有 29 种风格与 15 种提示词基础上，新增 Agent 工作流、风格本体/边界、10 个扩展风格候选、7 个机器可读视觉配方和质量验收规范。扩展条目与原始 29 种风格分开保存，避免未经完整核验就改变原始统计。

- `08-agent-visual-design-system.md`：任务路由、组合策略、提示词组装。
- `09-style-taxonomy-and-relations.md`：风格分类与概念边界。
- `10-visual-recipes.md` / `data/visual-recipes.json`：人工与机器可读配方。
- `11-design-evaluation.md`：验收标准。
- `data/style-relations.json`：风格类型和关系元数据。

## 使用方式

1. **找参考网站**：在 04-taxonomy.md 按领域或用途找站点，再到 01-sites.md 表一看推荐用途和核验状态。
2. **定风格**：用 02-styles.md 表二了解视觉特征，用 03-style-audience.md 判断是否匹配目标受众；需要组合时看 06-mixes.md。
3. **出图 / 出页面**：用 07-prompts.md 的提示词模板；网页 UI 可配合 awesome-design-md、styles.refero.design 的 DESIGN.md 约束 AI。
4. **程序读取**：用 data/kb.json 或 data/sites.csv、data/styles.csv，字段说明见 data/schema.md。

## 维护建议

- 每季度重跑一次链接检查，更新 data/verification.tsv 和各表的核验列。
- 新增网站时按表一字段补全，并写明来源与核验日期；新增受众结论时注明依据类型。
