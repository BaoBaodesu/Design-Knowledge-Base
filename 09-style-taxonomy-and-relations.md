---
title: "风格分类体系与关系图谱"
description: "定义风格类型、层级、关系与兼容规则，避免将艺术运动、审美潮流和制作技法混为一谈"
updated: 2026-11-26
tags: [taxonomy, ontology, style-relations]
---

# 风格分类体系与关系图谱

## 为什么需要分层

设计知识库中收录的概念并非同一种对象。包豪斯是历史设计运动，瑞士国际主义是平面设计体系，Y2K 是时代视觉美学，玻璃拟态是界面/材质表现，剪纸拼贴是图像制作技法。它们可以组合，但不能在概念定义上混为一谈。

## 推荐的多轴分类

每个条目可以同时拥有一个主类型和多个次级标签。

| style_type | 中文 | 定义 | 例子 |
|---|---|---|---|
| historical_movement | 历史艺术/设计运动 | 有明确历史语境、代表人物或组织 | Bauhaus、De Stijl、Constructivism、Art Nouveau、Art Deco、Pop Art |
| graphic_design_system | 平面设计体系 | 组织信息、字体、网格与版式的方法 | Swiss Style、Editorial Design、Brutalist Graphic Design |
| visual_aesthetic | 时代/数字视觉美学 | 特定时期或数字文化形成的视觉语言 | Y2K、Frutiger Aero、Vaporwave、Cyberpunk |
| visual_art_style | 视觉艺术风格 | 以图像表达、造型或观念为主 | Surrealism、Pop Art、Glitch Art |
| interface_style | 界面视觉风格 | 主要描述数字界面的层次、材质与交互外观 | Glassmorphism、Neumorphism、Flat Design |
| image_technique | 图像制作/印刷技法 | 描述素材如何制作、组合或复制 | Cut-out Collage、Photomontage、Risograph |
| material_language | 材质语言 | 描述表面属性与光学表现 | Chrome、Glass、Holographic、Paper Grain |
| composition_method | 构图方法 | 描述空间组织与视觉动线 | Grid、Asymmetry、Radial、Diagonal |
| typography_method | 字体/文字表现 | 描述文字如何成为视觉主体 | Kinetic Typography、Experimental Type |

## 关系类型

- `influenced_by`：历史影响或思想来源。需要可靠来源支持。
- `shares_visual_language_with`：视觉特征相似，不代表历史因果。
- `often_combined_with`：实践中可组合，属于经验建议。
- `contrasts_with`：构图/层级逻辑存在冲突，可通过分区解决。
- `uses_technique`：某风格常借用某制作技法。
- `has_material`：关联材质语言。
- `has_prompt_recipe`：存在可复用提示词配方。

## 重要边界与纠错

- **Art Deco ≠ Luxury Black & Gold**：Art Deco 是更广泛的装饰艺术设计运动；黑金只是常见配色/商业化演绎之一。
- **Brutalist architecture ≠ Brutalist graphic design ≠ Neo-brutalism UI**：三者有关联但不是同一个条目。现有 `brutal` 主要记录网页野兽派，应另建平面设计条目。
- **Y2K ≠ Frutiger Aero**：两者有时代交集，但前者常见金属、透明塑料、未来消费电子感；后者偏向清澈、自然、蓝绿、水滴、玻璃与乐观科技想象。
- **Glitch Art ≠ Cyberpunk**：故障艺术是数字图像表现方式，可用于赛博朋克，也可独立使用。
- **Surrealist Collage 与 Cut-out Collage 不同**：前者是观念/图像组合逻辑，后者是素材剪切与叠层技法。
- **Risograph** 是具体印刷工艺及其视觉美学，不应仅被理解成颗粒滤镜。

## 来源与参考图等级

| 等级 | 来源 | 主要用途 |
|---|---|---|
| T1 | 博物馆、档案馆、学术机构、艺术研究机构 | 历史、定义、作品 metadata、藏品图像 |
| T2 | 专业设计机构、设计出版物、一手设计规范 | 专业语境、制作方法、原始设计资料 |
| T3 | 艺术家或设计师作品页、专题研究项目、视觉参考社区 | 当代案例、术语使用、视觉参考 |

来源等级描述出版方与证据渠道。每条来源用 `supports[]` 标明它实际支持的字段，不能用机构权威替代逐条对应。当代数字美学没有 T1 定义来源时，记录当前证据缺口。

参考图至少记录 `title`、`creator`、`date`、`institution`、`page_url`、`rights`、`checked`。`image_url` 在机构提供直链时填写，具体许可信息见对应藏品页。

## 风格条目最低字段

```json
{
  "key": "stable-kebab-or-snake-key",
  "name": "中文名称",
  "name_en": "English name",
  "aliases": [],
  "style_type": "visual_aesthetic",
  "secondary_types": ["image_technique"],
  "historical_period": "年代、历史范围或当前证据缺口",
  "origin": "起源与背景，能够由 references 支持",
  "visual_signature": ["最具识别度的特征"],
  "layout": [],
  "geometry": [],
  "palette": [],
  "typography": [],
  "materials": [],
  "image_treatment": [],
  "lighting": [],
  "use_cases": [],
  "avoid_or_risks": [],
  "evidence_level": "有据|部分有据|经验观察",
  "evidence_notes": "说明参考来源与现代设计转译范围",
  "references": [
    {
      "title": "页面或作品名",
      "publisher": "机构或出版方",
      "tier": "T1|T2|T3",
      "url": "https://…",
      "supports": ["origin", "visual_signature"],
      "checked": "YYYY-MM-DD"
    }
  ],
  "reference_images": [
    {
      "title": "作品名",
      "creator": "创作者",
      "date": "作品年代",
      "institution": "收藏或发布机构",
      "page_url": "https://…",
      "image_url": "https://… 或 null",
      "rights": "版权、许可或权利核对入口",
      "checked": "YYYY-MM-DD"
    }
  ],
  "relations": []
}
```

## 当前知识库的推荐归类（主库 29 + 扩展层 10）

完整机器可读映射见 `data/style-relations.json` 的 `core_style_classifications`（主库 29 种）与 `entries[]`（扩展层 10 种）：

- 历史运动（`historical_movement`）：`bauhaus`、`memphis`（主库）；`constructivism`、`de_stijl`、`art_nouveau`、`art_deco`、`pop_art`（扩展层）。
- 平面体系（`graphic_design_system`）：`swiss`、`editorial`（主库）；`brutalist_graphic`（扩展层，与网页 `brutal` 分开）。
- 时代/数字美学（`visual_aesthetic`）：`y2k`、`cyber`、`vapor`、`japanese`、`guochao`、`luxury`、`organic`、`acid`、`retroweb`（主库）；`frutiger_aero`（扩展层）。
- 视觉艺术风格（`visual_art_style`）：`minimal`（主库）；`glitch_art`、`surrealist_collage`（扩展层）。
- 界面风格（`interface_style`）：`brutal`、`neobrutal`、`glass`、`neumorph`、`flat`、`skeuo`、`darkmode`、`webgl`（主库）。
- 图像技法（`image_technique`）：`riso`、`handdrawn`、`cinematic`（主库）；`cutout_collage`（扩展层）。
- 材质语言（`material_language`）：`clay`、`gradient`（主库）。
- 构图方法（`composition_method`）：`bento`（主库）。
- 字体/文字表现（`typography_method`）：`kinetic`（主库）。

## 注意

本分类用于 Agent 检索与决策；跨类别概念使用多标签并保留边界说明。
