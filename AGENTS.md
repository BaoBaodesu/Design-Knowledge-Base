# AGENTS.md — 设计师知识库使用说明（给 AI Agent）

本仓库是中文设计参考知识库（v1，2026-11-15）。用它来推荐参考网站、选择设计风格、判断受众匹配、组合风格、生成 AI 视觉提示词。回答用户时用中文。

## 1. 先读什么

1. `llms.txt`：全库索引，先读它了解有哪些文件。
2. `data/kb.json`：结构化全量数据，程序化检索的首选；字段见 `data/schema.md`。只需表格时可用 `data/sites.csv`、`data/styles.csv`。
3. 需要解释细节或引用原话时，再读对应 Markdown：
   - 网站：`01-sites.md`（表一，含逐站核验）
   - 风格：`02-styles.md`（表二 + 详解 + 网站×风格映射）
   - 受众：`03-style-audience.md`
   - 分类索引：`04-taxonomy.md`
   - 精选风格：`05-top10-styles.md`
   - 组合：`06-mixes.md`
   - 提示词：`07-prompts.md`
   - 来源：`sources.md`；研究过程：`notes/`

## 2. 按任务类型的检索路径

先确定任务类型、受众和平台，再按下表检索。表里的网站 id 对应 `kb.json` 的 `sites[].id`，风格 key 对应 `styles[].key`。

| 任务 | 先看风格（key） | 参考网站（id） | 再看 |
|---|---|---|---|
| 海报 | swiss、acid、riso、kinetic、bauhaus、memphis、guochao | Tokyo TDC(10)、D&AD(7)、One Show & ADC(8)、Fonts In Use(86)、Typewolf(85)、Savee(98)、It's Nice That(99)、Pinterest(95) | 03 受众 → 06 组合 → 07 提示词 |
| 品牌 / VI | minimal、swiss、editorial、luxury、organic、guochao | Brand New(100)、D&AD(7)、Savee(98)、Fonts In Use(86)、Logo Design Love(S14)、Behance(S1) | 03 受众 → 05 精选 |
| 网页 / UI | minimal、bento、glass、darkmode、neobrutal、webgl、flat | Awwwards(2)、Recent(59)、Siteinspire(60)、Land-book(61)、Landingfolio(62)、Mobbin(43)、Refero(45)、awesome-design-md(63)、Apple HIG(49)、Material 3(50)、Vercel Guidelines(51)、Impeccable(52) | 03 中 NN/g 的可用性结论；用 Vercel Guidelines / WCAG 自查 |
| 社媒内容 / 短视频 | kinetic、clay、y2k、gradient、neobrutal、acid | Motionographer(13)、Promonews(21)、Golden Wolf(25)、EyeCannndy(40)、Cosmos(97)、Pinterest(95) | 07 提示词；平台审美差异在 03 中标为推测 |
| 电商 | clay、guochao、organic、minimal、flat（Flat 2.0） | 花瓣(S4)、站酷(S3)、Landingfolio(62)、Mobbin(43)、Page Flows(44，结账/订阅流程)、Pinterest(95) | 原文 100 个里没有专门的电商站，需要说明这一点 |
| AI 出图 / AI 视频 | 任意风格，先在 07 找模板 | ShotDeck(36)、StillsLab(38)、Flim(39)、EyeCannndy(40)、StudioBinder(41)、Runway AIF(9)、styles.refero.design(S15) | 07 的「通用应用建议」 |

## 3. 风格 → 网站 → 提示词的关联查询

- **风格 → 网站**：`styles[key].site_ids`，或每个站点的 `sites[].style_keys` 反查。Markdown 里对应 `02-styles.md` 末尾的映射表和 `04-taxonomy.md` 的「按风格索引」。
- **风格 → 受众**：`styles[key].audience`（`who`、`mood`、`industries`、`avoid`、`regional_notes`、`basis`、`evidence`）。
- **风格 → 提示词**：`prompts[]` 中 `style_key` 相同的条目；`styles[key].has_prompt` 为 true 才有模板（共 15 种）。
- **风格 → 组合**：`mixes[]` 中 `primary` 或 `secondary` 等于该 key 的条目。
- **精选**：`styles[key].is_top10`，详情在 `top10[]`。
- 注意区分 `sites[].works_style`（收录作品的风格）和 `sites[].ui_style`（网站自身界面风格），两者经常不一样。

## 4. 核验状态字段

`sites[].verify`：
- `status_code`: `verified`（已核验：实际访问成功）、`partial`（部分核验：只拿到部分内容）、`failed`（访问失败）。
- `detail`：检查方法与结果原文；`checked`：检查日期（2026-11-15）。
- 推荐 `failed` 的站点时必须告诉用户它当前打不开，并给替代（如 Realtime Colors(92) → Coolors(91) + Radix Colors(93)）。`partial` 的站点要提示可能需要人工打开确认。
- 核验是某一天的快照；时间久了先提醒用户网站可能已变化。

`styles[].audience.evidence` 与 `mixes[].evidence`：`有据` / `部分有据` / `推测`。`sites[].source`: `article`（原文 100 个）或 `supplement`（文章之外补充）。

## 5. 推荐规则

- **必须解释理由**：每个推荐（风格、网站、组合）都要说明为什么适合这个任务和受众，引用具体字段（如视觉特征、适用场景、受众依据）。不要只列名字。
- **灵活组合，不照搬**：本库是参考，不是规定。根据用户的品牌、受众、平台和预算，从多个风格中取元素组合（参考 `06-mixes.md` 的主次比例思路），也可以提出库里没有的组合，但要说明这是你的判断。
- **给 2–3 个方向**：一般给出主推方案和备选方案，并说明各自的取舍和风险（`common_mistakes`、`avoid`、`risks`）。
- **如实转述推测**：标为「推测」或「部分有据」的受众判断、比例、地域差异，转述时要保留这个限定，例如「这是推测，没有数据支持」。不要把推测说成事实，也不要编造数字或来源。标为「据原文」「未核验」的数字同样要保留限定。
- **引用来源**：引用研究结论时附上 `references` / `sources.md` 中的链接（NN/g、维基百科、W3C 等）。
- **提示词**：用 07 的模板时替换 `[subject]` / `[主体]`，提醒用户 AI 生成的文字（尤其中文）需要后期替换，并检查对比度（WCAG 2.2 正文 ≥ 4.5:1）。

## 6. 禁止事项

- 禁止搜索、打开或引用 CSDN（csdn.net、blog.csdn.net）的任何内容。
- 不编造网站、数据、引用或核验结果；库里没有的信息，要么说明不知道，要么另行核验并注明来源与日期。
- 不要把「文章之外补充」的站点说成原文推荐。

## 7. 更新本库时

- 修改网站或风格数据时，同步更新 `data/kb.json`、对应 CSV 和 Markdown 表格，并更新 front matter 的 `updated`。
- 新的核验结果写入 `data/verification.tsv`，注明方法和日期。
