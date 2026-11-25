# AGENTS.md — 设计师知识库使用说明（给 AI Agent）

本仓库是中文设计参考知识库（v1，2026-11-22）。用它来推荐参考网站、选择设计风格、判断受众匹配、组合风格、生成 AI 视觉提示词。回答用户时用中文。

## 1. 先读什么

0. `08-agent-visual-design-system.md`：任务路由、风格选择、组合、提示词组装与验收流程（执行视觉设计任务时优先读）。
0. `09-style-taxonomy-and-relations.md`：风格类型、概念边界与关系类型。
0. `10-visual-recipes.md` 与 `data/visual-recipes.json`：扩展风格档案、可靠参考图与 16 个可复用视觉配方（JSON 为机器读取入口）。
0. `data/style-relations.json`：机器可读的扩展风格完整档案、分级来源、参考图、关系、边界说明及主库 29 种风格的 `core_style_classifications`。
0. `12-style-compatibility-and-composition.md` 与 `data/compatibility-matrix.json`：9×9 类型兼容矩阵、34 组风格对兼容表、维度所有权与 Agent 自主组合算法。
0. `data/extended-prompts.json`：16 种扩展与高频主库风格的模块化提示词（`modular_tokens`），支持按视觉维度拼装。
0. `11-design-evaluation.md`：视觉质量验收标准。

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

## 2. Agent 视觉设计工作流

- 先读 `08-agent-visual-design-system.md`，识别交付物、主体约束、受众、平台与画幅。
- 查 `data/kb.json` 获取现有风格，再查 `data/style-relations.json` 获取扩展档案、来源、参考图和边界；组合时查 `data/visual-recipes.json` 与 `10-visual-recipes.md`。
- 每次只选一个主风格，最多两个辅助风格。说明辅助风格具体作用于版式、几何、色彩、材质或图像技法中的哪一项。
- 历史运动、设计体系、数字美学、界面风格、图像技法不得当作同义概念。
- 角色任务先锁定身份特征，再做风格转译；重要文字建议后期排版。
- 按 `11-design-evaluation.md` 输出通过/部分通过/未通过，并指出证据和剩余风险。

## 3. 按任务类型的检索路径

先确定任务类型、受众和平台，再按下表检索。表里的网站 id 对应 `kb.json` 的 `sites[].id`，风格 key 对应 `styles[].key`。

| 任务 | 先看风格（key） | 参考网站（id） | 再看 |
|---|---|---|---|
| 海报 | swiss、acid、riso、kinetic、bauhaus、memphis、guochao | Tokyo TDC(10)、D&AD(7)、One Show & ADC(8)、Fonts In Use(86)、Typewolf(85)、Savee(98)、It's Nice That(99)、Pinterest(95) | 03 受众 → 06 组合 → 07 提示词 |
| 品牌 / VI | minimal、swiss、editorial、luxury、organic、guochao | Brand New(100)、D&AD(7)、Savee(98)、Fonts In Use(86)、Logo Design Love(S14)、Behance(S1) | 03 受众 → 05 精选 |
| 网页 / UI | minimal、bento、glass、darkmode、neobrutal、webgl、flat | Awwwards(2)、Recent(59)、Siteinspire(60)、Land-book(61)、Landingfolio(62)、Mobbin(43)、Refero(45)、awesome-design-md(63)、Apple HIG(49)、Material 3(50)、Vercel Guidelines(51)、Impeccable(52) | 03 中 NN/g 的可用性结论；用 Vercel Guidelines / WCAG 自查 |
| 社媒内容 / 短视频 | kinetic、clay、y2k、gradient、neobrutal、acid | Motionographer(13)、Promonews(21)、Golden Wolf(25)、EyeCannndy(40)、Cosmos(97)、Pinterest(95) | 07 提示词；平台审美差异在 03 中标为推测 |
| 电商 | clay、guochao、organic、minimal、flat（Flat 2.0） | 花瓣(S4)、站酷(S3)、Landingfolio(62)、Mobbin(43)、Page Flows(44，结账/订阅流程)、Pinterest(95) | 原文 100 个里没有专门的电商站，需要说明这一点 |
| AI 出图 / AI 视频 | 任意风格，先在 07 找模板 | ShotDeck(36)、StillsLab(38)、Flim(39)、EyeCannndy(40)、StudioBinder(41)、Runway AIF(9)、styles.refero.design(S15) | 07 的「通用应用建议」 |

## 4. 风格 → 网站 → 提示词的关联查询

- **风格 → 网站**：`styles[key].site_ids`，或每个站点的 `sites[].style_keys` 反查。Markdown 里对应 `02-styles.md` 末尾的映射表和 `04-taxonomy.md` 的「按风格索引」。
- **风格 → 受众**：`styles[key].audience`（`who`、`mood`、`industries`、`avoid`、`regional_notes`、`basis`、`evidence`）。
- **风格 → 提示词**：`prompts[]` 中 `style_key` 相同的条目；`styles[key].has_prompt` 为 true 才有模板（共 15 种）。
- **风格 → 组合**：`mixes[]` 中 `primary` 或 `secondary` 等于该 key 的条目。
- **精选**：`styles[key].is_top10`，详情在 `top10[]`。
- **扩展风格 → 来源与参考图**：`data/style-relations.json` 的 `entries[].references` 与 `reference_images`；按 `source_tiers` 选择证据，并检查 `supports`、`rights` 和 `checked`。
- 注意区分 `sites[].works_style`（收录作品的风格）和 `sites[].ui_style`（网站自身界面风格），两者经常不一样。

## 5. 核验状态字段

`sites[].verify`：
- `status_code`: `verified`（已核验：实际访问成功）、`partial`（部分核验：只拿到部分内容）、`failed`（访问失败）。
- `detail`：检查方法与结果原文；`checked`：检查日期（2026-11-15）。
- 推荐 `failed` 的站点时标注访问失败记录与核验日期，并给替代（如 Realtime Colors(92) → Coolors(91) + Radix Colors(93)）。`partial` 的站点注明已核验范围；任务依赖缺失内容时重新核验。
- 根据 `verify.checked` 判断网站信息的时效性；关键推荐或长期未复核的站点，先重新核验再引用。

`styles[].audience.evidence` 与 `mixes[].evidence`：`有据` / `部分有据` / `推测`。`sites[].source`: `article`（原文 100 个）或 `supplement`（文章之外补充）。

## 6. 推荐规则

- **必须解释理由**：每个推荐（风格、网站、组合）都要说明为什么适合这个任务和受众，引用具体字段（如视觉特征、适用场景、受众依据）。不要只列名字。
- **灵活组合**：根据用户的品牌、受众、平台和预算组合视觉元素，主次比例作为可调参数。库外组合标注为「Agent 提案」，并说明所借用的视觉维度。
- **给 2–3 个方向**：一般给出主推方案和备选方案，并说明各自的取舍和风险（`common_mistakes`、`avoid`、`risks`）。
- **证据表达**：根据 `evidence`、`verify` 和来源字段标注结论。`推测` 内容作为待验证假设；`部分有据` 内容区分来源支持与编者推断；「据原文」「未核验」保留来源属性。证据等级集中标注，不在每个句子重复限定。
- **引用来源**：引用研究结论时附上 `references` / `sources.md` 中的链接（NN/g、维基百科、W3C 等）。
- **提示词**：用 07 的模板时替换 `[subject]` / `[主体]`，提醒用户 AI 生成的文字（尤其中文）需要后期替换，并检查对比度（WCAG 2.2 正文 ≥ 4.5:1）。

## 7. 禁止事项

- 禁止搜索、打开或引用 CSDN（csdn.net、blog.csdn.net）的任何内容。
- 不编造网站、数据、引用或核验结果；库里没有的信息，要么说明不知道，要么另行核验并注明来源与日期。
- 不要把「文章之外补充」的站点说成原文推荐。

## 8. 更新本库时

- 修改网站或风格数据时，同步更新 `data/kb.json`、对应 CSV 和 Markdown 表格，并更新 front matter 的 `updated`。新增扩展风格时同时更新 `data/style-relations.json`、`data/visual-recipes.json`、`09-style-taxonomy-and-relations.md`、`10-visual-recipes.md` 与 `llms.txt`。
- 新的核验结果写入 `data/verification.tsv`，注明方法和日期。
