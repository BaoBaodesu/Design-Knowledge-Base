---
title: "风格兼容矩阵与 Agent 自主组合指南"
description: "定义 9×9 风格类型兼容规则、视觉维度所有权、风格对兼容表与 Agent 自主组合算法"
updated: 2026-11-26
tags: [compatibility, composition, agent, visual-design]
---

# 12 风格兼容矩阵与 Agent 自主组合指南

> 机器可读入口：`data/compatibility-matrix.json`；模块化提示词入口：`data/extended-prompts.json`；预设配方入口：`data/visual-recipes.json`。
> 本文件的兼容等级与权重比例作为 Agent 自主组合的初始工程规则，可按版面与出图效果灵活调整。

## 1. 为什么需要兼容矩阵

仅有预设配方（`R01–R16`）时，Agent 只能复用固定套路。引入**类型兼容矩阵 + 维度所有权 + 模块化提示词**后，Agent 可以面对任意用户需求，自主完成「选主风格 → 筛兼容辅助风格 → 分配视觉维度 → 抽取模块化提示词 → 冲突消解 → 验收」的完整闭环。

## 2. 自主组合 6 步算法（Agent 执行流程）

1. **解析交付物约束**：查 `data/compatibility-matrix.json` 的 `deliverable_constraints`，确定最大允许风格数（2–3 个）、视觉优先级和必选安全区（如角色海报先锁身份与安全区）。
2. **锁定唯一主风格（Primary，权重 60%–75%）**：按 `style_type` 从 `data/style-relations.json`（涵盖主库 29 + 扩展 10 = 39 种）检索最符合主视觉目标的风格，默认由它接管 `layout`、`geometry`、`typography`。
3. **查兼容矩阵筛辅助风格（Secondary，权重 20%–30%）**：
   - 先查 `style_pairs` 是否有明确条目（`recommended` / `conditional` / `conflict`）；
   - 若无显式条目，则按双方 `style_type` 查 `type_compatibility_matrix`（`synergy` / `zone_split` / `caution` / `avoid`）；
   - 遇到 `avoid` 或 `conflict` 时默认放弃或改换备选风格；遇到 `zone_split` 时必须声明空间分区方案。
4. **分配维度所有权（禁止平权平均混合）**：
   - 辅助风格 1 最多接管 **1–2 个非骨架维度**（如 `materials`、`image_treatment` 或 `palette`）；
   - 可选的第 3 风格（Accent，权重 5%–15%）最多接管 **1 个局部点缀维度**。
5. **模块化拼装提示词**：
   - 优先从 `data/extended-prompts.json` 的 `modular_tokens`（或 `data/kb.json` 的 `prompts[]`）按维度抽取 token；
   - 主风格取 `layout_tokens + geometry_tokens`；辅助风格仅取被分配槽位的 token（例如只取 `material_tokens`），**不要把两个风格的整段模板硬拼在一起**；
   - 合并双方 `negative` 与 `identity_guard`，再按 `08-agent-visual-design-system.md` 的 9 段式骨架组装。
6. **冲突自检与验收**：按 `11-design-evaluation.md` 检查主体一致性、风格纯度、对比度（WCAG 2.2）与伪文字风险。

## 3. 类型兼容矩阵速查（9 × 9）

| 主 \ 辅 | 历史运动 | 平面体系 | 数字美学 | 视觉艺术 | 界面风格 | 图像技法 | 材质语言 | 构图方法 | 字体表现 |
|---|---|---|---|---|---|---|---|---|---|
| **historical_movement** | caution | synergy | zone_split | caution | zone_split | synergy | synergy | synergy | synergy |
| **graphic_design_system** | synergy | caution | synergy | zone_split | synergy | synergy | synergy | synergy | synergy |
| **visual_aesthetic** | zone_split | synergy | caution | zone_split | synergy | synergy | synergy | synergy | synergy |
| **visual_art_style** | caution | zone_split | zone_split | avoid | zone_split | synergy | synergy | synergy | zone_split |
| **interface_style** | zone_split | synergy | synergy | zone_split | avoid | zone_split | synergy | synergy | synergy |
| **image_technique** | synergy | synergy | synergy | synergy | zone_split | caution | synergy | synergy | synergy |
| **material_language** | synergy | synergy | synergy | synergy | synergy | synergy | avoid | synergy | synergy |
| **composition_method** | synergy | synergy | synergy | synergy | synergy | synergy | synergy | avoid | synergy |
| **typography_method** | synergy | synergy | synergy | zone_split | synergy | synergy | synergy | synergy | avoid |

## 4. 三大冲突消解模式

1. **空间分区（Zone Split）**：理性网格（`swiss` / `editorial` / `de_stijl`）负责标题、编号与信息区；表现性风格（`cutout_collage` / `surrealist_collage` / `acid` / `art_nouveau`）负责中心主体或画框内部。
2. **层级隔离（Layer Isolation）**：人脸、关键配饰与正文文字留在清晰前景层；`glitch_art` 切片、`pop_art` 网点、`riso` 套印偏移仅施加于背景与边缘层。
3. **色板收敛（Palette Lock）**：无论组合几种风格，全画面主色不超过 3–4 个、强调色不超过 1 个，防止每个风格各自带入一套冲突配色。

## 5. 典型高冲突禁忌（默认避免）

- `glass` × `neobrutal`：半透明柔和毛玻璃与粗黑硬描边/硬投影在 UI 语言上直接冲突。
- `neumorph` × `brutal`：低对比柔和浮雕与高反差原始网页直接互斥。
- `frutiger_aero` × `cyber`：清澈乐观日光水滴与暗黑反乌托邦霓虹直接对立。
- `constructivism` × `art_nouveau`：工业锋利对角线与柔和有机藤蔓曲线在几何与理念上完全冲突。
- `art_nouveau` × `de_stijl`：有机流动曲线与严格正交矩形网格直接对立（除非做极端内外分区实验）。
