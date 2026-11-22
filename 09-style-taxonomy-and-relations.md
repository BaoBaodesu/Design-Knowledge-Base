---
title: "风格分类体系与关系图谱"
description: "定义风格类型、层级、关系与兼容规则，避免将艺术运动、审美潮流和制作技法混为一谈"
updated: 2026-11-22
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

## 风格条目最低字段

```json
{
  "key": "stable-kebab-or-snake-key",
  "name": "中文名称",
  "name_en": "English name",
  "style_type": "visual_aesthetic",
  "secondary_types": ["image_technique"],
  "historical_period": "年代或未核验",
  "origin": "起源与背景，附来源或标记未核验",
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
  "relations": [],
  "evidence_level": "有据|部分有据|编者归纳|未核验",
  "references": []
}
```

## 当前知识库的推荐归类

- 历史运动：Bauhaus、Memphis、Art Deco（建议拆分）、Art Nouveau（新增）、De Stijl（新增）、Constructivism（新增）、Pop Art（新增）。
- 平面体系：Swiss、Editorial、Brutalist Graphic Design（新增，与现有 web brutal 分开）。
- 数字美学：Y2K、Vaporwave、Cyberpunk、Frutiger Aero（新增）。
- 数字表现：Glitch Art（新增）。
- 图像技法：Risograph、Cut-out Collage（新增）、Surrealist Collage（新增，兼具视觉艺术分类）。
- 界面风格：Glassmorphism、Neumorphism、Flat、Skeuomorphism、Bento（Bento 更适合作为布局模式）。
- 构图/文字方法：Kinetic Typography、Grid、Bento Grid。

## 注意

本分类是为 Agent 检索和决策服务的实用本体，不是艺术史学界唯一或权威的分类法。对于跨类别概念，允许多标签并保留边界说明。
