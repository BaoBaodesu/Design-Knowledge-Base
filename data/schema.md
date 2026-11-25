# data/ 字段说明

更新日期：2026-11-25。所有文本为中文（zh-Hans），文件编码 UTF-8。

## kb.json 顶层

| 字段 | 类型 | 说明 |
|---|---|---|
| `meta` | object | 标题、版本、更新日期、来源、计数、证据等级与核验状态的取值说明、研究规范 |
| `sites` | array | 115 个网站（100 个原文 + 15 个补充） |
| `styles` | array | 29 种风格（含受众信息） |
| `top10` | array | 精选 10 大风格补充信息 |
| `mixes` | array | 14 个混合风格方案 |
| `prompts` | array | 15 种风格的提示词模板 |

## sites[]

| 字段 | 类型 | 说明 |
|---|---|---|
| `id` | string | 原文编号 `"1"`–`"100"`；补充站为 `"S1"`–`"S15"` |
| `source` | string | `article`（原文）或 `supplement`（文章之外补充） |
| `name` / `url` | string | 网站名称、链接 |
| `category` | string | 原文九类之一；补充站为「文章之外补充」 |
| `main` | string | 主要内容 |
| `resource_type` | string | 资源类型（如 奖项/网页灵感、截图库/UI） |
| `works_style` | string | 收录作品的风格与设计特点（编者归纳） |
| `ui_style` | string | 网站自身界面风格（2026-11-15 首页截图观察） |
| `scene` | string | 适用场景（补充站可能为空） |
| `recommended_use` | string | 推荐用途 |
| `domains` | string[] | 领域标签（网页、UI、动态、3D、影视、字体、配色、品牌等） |
| `style_keys` | string[] | 关联风格，对应 `styles[].key` |
| `paid` | bool / null | 原文是否标注付费；补充站为 null（未判断） |
| `verify.status` | string | 已核验 / 部分核验 / 访问失败 |
| `verify.status_code` | string | `verified` / `partial` / `failed` |
| `verify.detail` | string | 检查方法与结果 |
| `verify.checked` | string | 检查日期 |

## styles[]

| 字段 | 类型 | 说明 |
|---|---|---|
| `key` | string | 风格唯一键（如 `swiss`、`bento`、`guochao`） |
| `name` / `name_en` | string | 中文名 / 英文名 |
| `origin` | string | 起源与背景（注明出处或「未核验」） |
| `colors`、`typography`、`layout`、`graphics`、`texture` | string | 配色、字体、版式构图、图形元素、质感 |
| `common_mistakes` | string | 常见误区 |
| `references` | {label,url}[] | 参考来源（2026-11-15 已验证可访问） |
| `audience.who` | string | 受众假设（年龄/职业/兴趣）；证据等级统一由 `audience.evidence` 记录，不在文本中重复标注 |
| `audience.mood` | string | 情绪与品牌印象 |
| `audience.industries` | string | 适合行业/用途 |
| `audience.avoid` | string | 使用边界与需重点验证的场景 |
| `audience.regional_notes` | string | 地域/文化/平台观察；证据等级由 `audience.evidence` 记录 |
| `audience.basis` | string | 判断依据 |
| `audience.evidence` | string | `有据` / `部分有据` / `推测` |
| `site_ids` | string[] | 关联网站 id |
| `is_top10` | bool | 是否精选 10 大风格 |
| `has_prompt` | bool | 是否有提示词模板 |

## top10[]

`rank`、`key`（对应 styles）、`core`（核心特征）、`strengths`（优势）、`limits`（局限）。

## mixes[]

`id`、`name`、`primary` / `secondary`（风格 key）、`ratio`（主:次，可调的初始参数）、`logic`、`visual`、`scenarios`、`risks`、`evidence`（当前均为「推测」）。

## prompts[]

`style_key`、`subject_example`、`style_en`、`style_zh`、`composition` / `lighting` / `palette` / `negative`（格式为「英文 / 中文」）、`compatibility`（适配模型）、`tips`（应用建议）。

## CSV

- `sites.csv`：列与 `sites[]` 对应；数组字段（`domains`、`style_keys`）用 `;` 分隔；`verify_status` 为 `status_code`。
- `styles.csv`：风格核心字段 + `audience`、`industries`、`avoid`、`evidence`；`site_ids`、`reference_urls` 用 `;` 分隔。

## 其他文件

- `verification.tsv`：`id, name, url, curl_status, final_url, verdict, detail, checked`。
- `article-100-list.json`：原文清单，字段 `n`（编号）、`name`、`url`、`desc`（原文摘要）、`sec`（原文分类）、`paid`。
- `screenshots/sheet_00–09.webp`：首页截图拼图，左上角红标为网站 id。


## Agent 视觉设计扩展数据（2026-11-25）

- `data/style-relations.json`：`source_tiers` 定义 T1–T3 来源等级；`entries[]` 包含 10 个扩展风格的名称、别名、类型、时期、起源、视觉维度、用途、风险、证据说明、分级来源、参考图与关系；`core_style_classifications` 为主库 29 种风格提供机器可读的 `style_type` 与 `secondary_types` 映射。`references[]` 用 `supports[]` 标记证据对应字段；`reference_images[]` 记录作品页、创作者、机构、权利与核验日期。扩展条目不计入原始 `styles[]` 29 条统计。
- `data/visual-recipes.json`：`recipes[]`（共 16 条，R01–R16）统一包含 `id`、`name`、`primary`、`secondary[]`、`deliverables[]`、`layout`、`geometry[]`、`palette[]`、`materials[]`、`risks[]`、`prompt`、`reference_pages[]`；R01 另有 `aliases[]`。
- `data/compatibility-matrix.json`：包含 `type_compatibility_matrix`（9×9 类型兼容矩阵）、`dimension_ownership_rules`（主/辅/点缀权重与维度槽位规则）、`deliverable_constraints`（6 类交付物约束）与 `style_pairs[]`（34 组具体风格对兼容规则及关联 `recipe_id`）。
- `data/extended-prompts.json`：`prompts[]`（共 16 条，覆盖 10 个扩展风格 + 6 个高频主库风格）除兼容 `kb.json` 的基础字段外，新增 `source_layer` 与 `modular_tokens`（`layout_tokens`、`geometry_tokens`、`palette_tokens`、`material_tokens`、`treatment_tokens`、`lighting_tokens`、`identity_guard`），支持 Agent 按维度拼装提示词。
- 类型本体定义与使用规则见 `09-style-taxonomy-and-relations.md`；Agent 路由见 `08-agent-visual-design-system.md`；自主组合与兼容矩阵见 `12-style-compatibility-and-composition.md`；验收规则见 `11-design-evaluation.md`。
