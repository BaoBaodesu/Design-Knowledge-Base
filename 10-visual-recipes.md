---
title: "可复用视觉设计配方"
description: "将风格知识转化为任务导向的视觉配方，包含构图、色彩、材质、提示词骨架和风险"
updated: 2026-11-22
tags: [recipes, posters, character-design, prompt-engineering]
---

# 可复用视觉设计配方

> 配方是 Agent 的起点，不是固定模板。比例为初始视觉权重建议，属于编者经验，不是研究结论。

## A. 风格补充清单

| key | 名称 | 类型 | 视觉签名 | 推荐用途 |
|---|---|---|---|---|
| constructivism | 俄罗斯构成主义 | historical_movement | 对角线、红黑白、放射构图、粗体文字 | 力量感海报、活动视觉 |
| de_stijl | 风格派 | historical_movement | 水平/垂直线、矩形色块、有限原色 | 抽象构成、极简角色卡 |
| art_nouveau | 新艺术运动 | historical_movement | 有机曲线、植物纹样、装饰边框、人物与背景融合 | 幻想肖像、角色立绘 |
| art_deco | 装饰艺术 | historical_movement | 阶梯纹、扇形、放射几何、金属装饰 | 奢华角色海报、封面 |
| pop_art | 波普艺术 | historical_movement | 漫画网点、粗轮廓、重复图像、强对比色 | Q版角色、漫画海报 |
| frutiger_aero | Frutiger Aero | visual_aesthetic | 蓝绿、玻璃、水滴、气泡、自然与科技融合 | AI 助手、清新科技角色 |
| glitch_art | 故障艺术 | visual_art_style | RGB 分离、扫描线、像素错位、数据破损 | 数字角色、音乐视觉 |
| surrealist_collage | 超现实主义拼贴 | visual_art_style | 尺度错置、不可能空间、隐喻式物体组合 | 概念海报、专辑封面 |
| cutout_collage | 剪纸拼贴 | image_technique | 剪影、撕纸边缘、纸张叠层、遮挡 | 角色拼贴、独立出版 |
| brutalist_graphic | 野兽派平面设计 | graphic_design_system | 原始排版、粗重字体、强烈裁切、粗糙结构 | 实验海报、反商业视觉 |

## B. 组合配方

### R01 — Swiss Grid × Bauhaus Geometry × Y2K Cyber Fashion

- 主目标：角色主视觉与现代科技时尚感并存。
- 构图：瑞士网格负责信息区；人物区域允许非对称穿插。
- 几何：将发束、衣摆、肩线抽象成矩形、三角、圆弧模块，但保留人物轮廓。
- 色彩：深炭灰/冷白为底，钴蓝或冰青为强调色，银色只做材质点缀。
- 材质：局部铬金属、透明塑料、镭射反射；不要全画面金属化。
- 字体：大号无衬线标题 + 小号编号/注释；中文文字后期排版。
- 风险：网格与自由拼贴冲突。用分区而不是平均混合解决。
- Prompt skeleton: `character editorial poster, Swiss grid typography, Bauhaus geometric decomposition, Y2K cyber fashion accents, asymmetric layout, restrained chrome and translucent materials, preserve original character identity`.

### R02 — Art Nouveau × Art Deco × Fantasy Portrait

- 主目标：典雅、装饰性强、具有收藏肖像感。
- 构图：中心人物肖像，外围有机曲线边框；用 Art Deco 的阶梯/扇形结构建立边界。
- 色彩：古金、墨绿、酒红、象牙白；避免所有元素都使用金色。
- 材质：纸张、金箔、珐琅、细腻印刷纹理。
- 风险：边框过度复杂会压迫人物；人物脸部保持清晰。
- Prompt skeleton: `ornate fantasy character portrait, Art Nouveau organic floral framing, Art Deco geometric symmetry, refined antique gold accents, elegant negative space, preserve character identity`.

### R03 — Pop Art × Risograph × Comic Collage

- 主目标：活泼、直接、强识别度。
- 构图：漫画分格或重复人物，主体与对话气泡分离。
- 色彩：限制在 3–5 个专色，允许套印错位。
- 材质：半色调网点、纸张颗粒、油墨叠色。
- 风险：网点不能覆盖眼睛、嘴部等表情关键区；文字最好后期制作。
- Prompt skeleton: `playful character poster, Pop Art comic halftone, Risograph spot-color overprint, bold outlines, layered comic collage, expressive pose`.

### R04 — Constructivism × Brutalist Graphic

- 主目标：强烈、直接、具有运动感。
- 构图：单一主对角线或放射结构；大字作为图形，不要同时出现多个竞争焦点。
- 色彩：红、黑、白，最多增加一个强调色。
- 材质：纸张印刷、油墨磨损、轻微套色偏移。
- 风险：不要把所有元素倾斜；保持清晰的阅读方向。
- Prompt skeleton: `constructivist graphic poster, bold diagonal composition, red black cream palette, monumental typography, brutalist editorial structure, print grain`.

### R05 — Frutiger Aero × Glassmorphism

- 主目标：清澈、友好、乐观的未来科技感。
- 构图：大面积通透背景，少量漂浮玻璃物体，主体有足够呼吸空间。
- 色彩：天蓝、青绿、白色；控制彩虹渐变使用面积。
- 材质：透明玻璃、水滴、液体、柔和高光。
- 风险：玻璃拟态面板不能牺牲文字对比；避免过度模糊。
- Prompt skeleton: `optimistic futuristic visual, Frutiger Aero aesthetic, clear blue sky and aqua green, translucent glass bubbles, water droplets, soft sunlight, clean readable composition`.

### R06 — Surrealist Collage × Editorial Design

- 主目标：有概念、有叙事的艺术海报。
- 构图：杂志网格负责信息，超现实主体打破局部空间逻辑。
- 元素：选择一个核心隐喻物体，最多两个次级异质物体。
- 色彩：由主题决定，限制主色数量。
- 风险：不要随机堆砌素材；所有错位应服务一个可解释的概念。
- Prompt skeleton: `surrealist editorial collage, impossible scale relationships, conceptual visual metaphor, refined magazine grid, controlled negative space, tactile photographic cutouts`.

### R07 — Cut-out Collage × Swiss Typography

- 主目标：角色素材拆分后仍保持清晰、时尚的版式。
- 构图：人物剪影分层，标题按网格对齐；局部撕纸边缘形成节奏。
- 材质：纸张、扫描纹理、胶带、套印偏移。
- 风险：剪切边缘不能破坏头发、手指和服装轮廓。
- Prompt skeleton: `layered cut-paper character collage, Swiss editorial typography, torn paper edges, precise grid, overlapping cutout shapes, preserve silhouette and facial identity`.

## C. 角色海报配方通用约束

- 身份锁定：保留发型、发色、瞳色、脸型、服装轮廓、配饰与角色标志。
- 画面层级：人物 > 主标题 > 次级信息 > 装饰。
- 文字准确性：模型生成文字不作为最终排版依据。
- 视觉密度：每个区域只允许一个主导逻辑；不要让网格、拼贴、装饰边框同时争夺主导。
- 适配性：人物立绘、海报、封面和 UI 需要不同的版式方案，不可直接复用同一提示词。
