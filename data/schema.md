# data/ 字段说明

更新日期：2026-11-15。所有文本为中文（zh-Hans），文件编码 UTF-8。

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
| `audience.who` | string | 潜在受众（年龄/职业/兴趣） |
| `audience.mood` | string | 情绪与品牌印象 |
| `audience.industries` | string | 适合行业/用途 |
| `audience.avoid` | string | 不适合场景 |
| `audience.regional_notes` | string | 地域/文化/平台差异 |
| `audience.basis` | string | 判断依据 |
| `audience.evidence` | string | `有据` / `部分有据` / `推测` |
| `site_ids` | string[] | 关联网站 id |
| `is_top10` | bool | 是否精选 10 大风格 |
| `has_prompt` | bool | 是否有提示词模板 |

## top10[]

`rank`、`key`（对应 styles）、`core`（核心特征）、`strengths`（优势）、`limits`（局限）。

## mixes[]

`id`、`name`、`primary` / `secondary`（风格 key）、`ratio`（主:次，推测）、`logic`、`visual`、`scenarios`、`risks`、`evidence`（均为「推测」）。

## prompts[]

`style_key`、`subject_example`、`style_en`、`style_zh`、`composition` / `lighting` / `palette` / `negative`（格式为「英文 / 中文」）、`compatibility`（适配模型）、`tips`（应用建议）。

## CSV

- `sites.csv`：列与 `sites[]` 对应；数组字段（`domains`、`style_keys`）用 `;` 分隔；`verify_status` 为 `status_code`。
- `styles.csv`：风格核心字段 + `audience`、`industries`、`avoid`、`evidence`；`site_ids`、`reference_urls` 用 `;` 分隔。

## 其他文件

- `verification.tsv`：`id, name, url, curl_status, final_url, verdict, detail, checked`。
- `article-100-list.json`：原文清单，字段 `n`（编号）、`name`、`url`、`desc`（原文摘要）、`sec`（原文分类）、`paid`。
- `screenshots/sheet_00–09.webp`：首页截图拼图，左上角红标为网站 id。
