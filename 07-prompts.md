---
title: "AI 视觉提示词模板"
description: "15 种风格的中英文提示词模板（主体+风格+构图+光线+配色+负面词），适配 Midjourney / Stable Diffusion / 通用，附应用建议"
updated: 2026-11-15
tags: [prompts, ai-image, midjourney, stable-diffusion, design-kb]
---

# 07 AI 视觉提示词模板与应用建议

> 结构：主体占位符 + 风格词 + 构图 + 光线 + 配色 + 负面词。中括号内替换为你的主体。
> 适配说明：Midjourney 负面词用 `--no`；Stable Diffusion 负面词放 Negative prompt；其他工具（如通用文生图）直接用自然语言。Midjourney 参数（如 `--ar` 画幅、`--style raw`）以当前版本官方文档为准（未逐一核验版本差异）。

## 通用应用建议
- 先用本库网站找 3–5 张参考图，确定风格名称再写提示词（原文作者建议：叫得出风格名称、说得清手法，AI 输出质量明显更高）。
- 网页/UI 类：在编码 AI 中用 awesome-design-md 或 styles.refero.design 的 DESIGN.md 约束风格，用 Vercel Guidelines 与 Impeccable 自查。
- 视频/镜头类：用 StudioBinder、EyeCannndy 的术语（low angle、dolly in、whip pan）描述镜头。
- AI 生成的文字（尤其中文）经常出错：标题文字后期在设计软件中替换。
- 落地前检查对比度（WCAG 2.2 正文 ≥ 4.5:1）。

## 极简主义（Minimalism）　★精选
- 主体占位符示例：[主体：如 一款白色无线耳机]
- 适配：通用（MJ/SD/其他）

**英文模板**
```
[subject], minimalist design, clean composition, generous negative space, refined typography, Swiss-inspired restraint, centered subject, rule of thirds, lots of empty space, soft diffused studio light, monochrome palette, off-white and charcoal with one accent color
```
**中文模板**
```
[主体：如 一款白色无线耳机]，极简主义，干净构图，大量留白，精致排版，主体居中或三分法，大面积留白，柔和漫射棚拍光，黑白灰+单一强调色
```
**负面词**：EN `clutter, busy background, multiple subjects, text artifacts, gradients overload`｜中文 杂乱、背景复杂、多主体、乱码文字

**Midjourney 示例**
```
[subject], minimalist design, clean composition, generous negative space, refined typography, Swiss-inspired restraint, centered subject, rule of thirds, lots of empty space, soft diffused studio light, monochrome palette, off-white and charcoal with one accent color --ar 3:4 --no clutter, busy background
```
**SD 写法**：Positive = 英文模板；Negative = `clutter, busy background, multiple subjects, text artifacts, gradients overload, lowres, blurry, watermark`

- 应用建议：先确定唯一主体与一个强调色；海报类加 'poster layout, grid' 引导版式

## 瑞士国际主义（International Typographic Style / Swiss Style）　★精选
- 主体占位符示例：[主体：如 爵士音乐节海报]
- 适配：MJ 更擅长海报版式；SD 建议配合 ControlNet 布局

**英文模板**
```
[subject], International Typographic Style poster, strict modular grid, bold sans-serif headline, asymmetric layout, objective photography, flat color blocks, asymmetric grid layout, strong left alignment, flat even lighting, white, black and signal red
```
**中文模板**
```
[主体：如 爵士音乐节海报]，瑞士国际主义海报，严格模块网格，粗体无衬线大标题，非对称版式，非对称网格，强左对齐，平光，白、黑、信号红
```
**负面词**：EN `3D render, ornate decoration, script fonts, gradients, distorted text`｜中文 3D渲染、繁复装饰、手写体、渐变、扭曲文字

**Midjourney 示例**
```
[subject], International Typographic Style poster, strict modular grid, bold sans-serif headline, asymmetric layout, objective photography, flat color blocks, asymmetric grid layout, strong left alignment, flat even lighting, white, black and signal red --ar 3:4 --no 3D render, ornate decoration
```
**SD 写法**：Positive = 英文模板；Negative = `3D render, ornate decoration, script fonts, gradients, distorted text, lowres, blurry, watermark`

- 应用建议：AI 生成文字常出错：标题文字建议后期在设计软件中替换

## 杂志编辑风（Editorial Design）　★精选
- 主体占位符示例：[主体：如 一篇关于城市慢生活的专题]
- 适配：通用

**英文模板**
```
[subject], editorial magazine layout, serif headline, multi-column grid, large photography, pull quotes, print texture, magazine spread composition, image and text interplay, natural window light photography, cream paper, black ink, one accent color
```
**中文模板**
```
[主体：如 一篇关于城市慢生活的专题]，杂志编辑风版式，衬线大标题，多栏网格，大幅摄影，引言，跨页构图，图文穿插，自然窗光摄影，米白纸色、黑墨、一种强调色
```
**负面词**：EN `cluttered UI, neon, cartoon, low resolution`｜中文 杂乱界面、霓虹、卡通、低清

**Midjourney 示例**
```
[subject], editorial magazine layout, serif headline, multi-column grid, large photography, pull quotes, print texture, magazine spread composition, image and text interplay, natural window light photography, cream paper, black ink, one accent color --ar 3:4 --no cluttered UI, neon
```
**SD 写法**：Positive = 英文模板；Negative = `cluttered UI, neon, cartoon, low resolution, lowres, blurry, watermark`

- 应用建议：适合生成版式草图与配图；正文务必用真实文字重排

## 新野兽派（Neo-brutalism）　★精选
- 主体占位符示例：[主体：如 一款记账 App 落地页]
- 适配：通用；UI 概念图建议 --ar 16:9 / 9:16

**英文模板**
```
[subject], neo-brutalism UI, thick black outlines, hard offset drop shadows, bold flat colors, chunky sans-serif, playful blocky layout, blocky card grid, slightly tilted stickers, flat lighting, no gradients, bright yellow, hot pink, cobalt blue with pure black
```
**中文模板**
```
[主体：如 一款记账 App 落地页]，新野兽派界面，粗黑描边，硬投影偏移，大胆纯色，粗体无衬线，块状布局，块状卡片网格，略倾斜的贴纸元素，平光无渐变，亮黄、桃粉、钴蓝+纯黑
```
**负面词**：EN `soft shadows, glassmorphism, photorealism, gradients`｜中文 柔和阴影、玻璃拟态、写实、渐变

**Midjourney 示例**
```
[subject], neo-brutalism UI, thick black outlines, hard offset drop shadows, bold flat colors, chunky sans-serif, playful blocky layout, blocky card grid, slightly tilted stickers, flat lighting, no gradients, bright yellow, hot pink, cobalt blue with pure black --ar 3:4 --no soft shadows, glassmorphism
```
**SD 写法**：Positive = 英文模板；Negative = `soft shadows, glassmorphism, photorealism, gradients, lowres, blurry, watermark`

- 应用建议：生成后检查对比度与可点击元素是否可辨

## Bento 网格（Bento Grid）　★精选
- 主体占位符示例：[主体：如 AI 笔记应用功能介绍页]
- 适配：通用

**英文模板**
```
[subject], bento grid layout, rounded cards of varying sizes, clean product UI, large numbers, subtle borders, Apple keynote style, modular bento box grid, one hero card, soft studio light, subtle inner glow, neutral light gray background with one dark card and one accent
```
**中文模板**
```
[主体：如 AI 笔记应用功能介绍页]，Bento 网格布局，大小不一的圆角卡片，简洁产品界面，大数字，细描边，模块化便当网格，一张主卡，柔光+轻微内发光，浅灰底+一张深色卡+一个强调色
```
**负面词**：EN `cluttered, uneven gaps, overlapping cards, illegible text`｜中文 杂乱、间距不一、卡片重叠、文字难读

**Midjourney 示例**
```
[subject], bento grid layout, rounded cards of varying sizes, clean product UI, large numbers, subtle borders, Apple keynote style, modular bento box grid, one hero card, soft studio light, subtle inner glow, neutral light gray background with one dark card and one accent --ar 3:4 --no cluttered, uneven gaps
```
**SD 写法**：Positive = 英文模板；Negative = `cluttered, uneven gaps, overlapping cards, illegible text, lowres, blurry, watermark`

- 应用建议：明确卡片数量（如 6–8 张）与主卡位置；文字后期替换

## 玻璃拟态（Glassmorphism）　★精选
- 主体占位符示例：[主体：如 智能家居控制面板]
- 适配：通用；SD 可加 'ui design, dribbble' 类风格词

**英文模板**
```
[subject], glassmorphism UI, frosted translucent panels, background blur, soft highlights, vibrant gradient background, depth layers, layered floating panels, soft rim light, purple-blue-pink gradient backdrop, white translucent glass
```
**中文模板**
```
[主体：如 智能家居控制面板]，玻璃拟态界面，磨砂半透明面板，背景模糊，柔和高光，鲜艳渐变背景，层叠漂浮面板，柔和轮廓光，紫蓝粉渐变底+白色半透明玻璃
```
**负面词**：EN `low contrast text, flat design, harsh shadows`｜中文 低对比文字、扁平、硬阴影

**Midjourney 示例**
```
[subject], glassmorphism UI, frosted translucent panels, background blur, soft highlights, vibrant gradient background, depth layers, layered floating panels, soft rim light, purple-blue-pink gradient backdrop, white translucent glass --ar 3:4 --no low contrast text, flat design
```
**SD 写法**：Positive = 英文模板；Negative = `low contrast text, flat design, harsh shadows, lowres, blurry, watermark`

- 应用建议：落地时用 WCAG 对比度工具检查文字

## 深色科技风（Dark Mode / Dark Tech）　★精选
- 主体占位符示例：[主体：如 开发者数据分析仪表盘]
- 适配：通用

**英文模板**
```
[subject], dark mode tech interface, near-black background, thin borders, subtle glow, grid backdrop, crisp data visualization, dashboard grid with clear hierarchy, subtle ambient glow, #0A0A0A background, gray text, one cyan or violet accent
```
**中文模板**
```
[主体：如 开发者数据分析仪表盘]，深色科技界面，近黑背景，细描边，微光，网格背景，清晰数据可视化，层级清晰的仪表盘网格，微弱环境光，近黑底、灰字、一个青或紫强调色
```
**负面词**：EN `pure white on pure black glare, neon overload, clutter`｜中文 纯白纯黑强烈眩光、霓虹过量、杂乱

**Midjourney 示例**
```
[subject], dark mode tech interface, near-black background, thin borders, subtle glow, grid backdrop, crisp data visualization, dashboard grid with clear hierarchy, subtle ambient glow, #0A0A0A background, gray text, one cyan or violet accent --ar 3:4 --no pure white on pure black glare, neon overload
```
**SD 写法**：Positive = 英文模板；Negative = `pure white on pure black glare, neon overload, clutter, lowres, blurry, watermark`

- 应用建议：避免纯黑+纯白；强调色只用一种

## 3D / 黏土风（3D Clay / Soft 3D）　★精选
- 主体占位符示例：[主体：如 一只抱着手机的小熊吉祥物]
- 适配：MJ/SD 均可；SD 可配合 3D/clay LoRA（需自行核验授权）

**英文模板**
```
[subject], 3D clay style, soft rounded shapes, matte plasticine texture, cute character, pastel colors, isometric or centered, centered hero object, floating elements, soft global illumination, subtle subsurface scattering, pastel pink, mint, lavender, cream
```
**中文模板**
```
[主体：如 一只抱着手机的小熊吉祥物]，3D 黏土风，柔和圆润造型，哑光橡皮泥质感，可爱角色，马卡龙色，主体居中，漂浮元素，柔和全局光照+轻次表面散射，粉、薄荷绿、薰衣草紫、奶油色
```
**负面词**：EN `photorealistic, sharp edges, glossy plastic, dark mood`｜中文 写实、尖锐边缘、亮面塑料、暗调

**Midjourney 示例**
```
[subject], 3D clay style, soft rounded shapes, matte plasticine texture, cute character, pastel colors, isometric or centered, centered hero object, floating elements, soft global illumination, subtle subsurface scattering, pastel pink, mint, lavender, cream --ar 3:4 --no photorealistic, sharp edges
```
**SD 写法**：Positive = 英文模板；Negative = `photorealistic, sharp edges, glossy plastic, dark mood, lowres, blurry, watermark`

- 应用建议：保持角色一致性：固定种子或使用参考图功能

## Y2K 千禧风（Y2K aesthetic）　★精选
- 主体占位符示例：[主体：如 美妆品牌新品海报]
- 适配：MJ 风格化更强；通用

**英文模板**
```
[subject], Y2K aesthetic, chrome metallic typography, bubbly shapes, sparkles, early-2000s interface elements, iridescent, centered collage, floating objects, glossy reflections, lens flare, icy blue, silver, baby pink, lilac
```
**中文模板**
```
[主体：如 美妆品牌新品海报]，Y2K 千禧风，铬金属字体，气泡形状，星光闪烁，千禧年界面元素，镭射彩虹光，居中拼贴，漂浮物体，光泽反射、镜头光晕，冰蓝、银、婴儿粉、淡紫
```
**负面词**：EN `muted earthy tones, minimal, realistic photography`｜中文 低饱和大地色、极简、写实摄影

**Midjourney 示例**
```
[subject], Y2K aesthetic, chrome metallic typography, bubbly shapes, sparkles, early-2000s interface elements, iridescent, centered collage, floating objects, glossy reflections, lens flare, icy blue, silver, baby pink, lilac --ar 3:4 --no muted earthy tones, minimal
```
**SD 写法**：Positive = 英文模板；Negative = `muted earthy tones, minimal, realistic photography, lowres, blurry, watermark`

- 应用建议：注意与品牌调性匹配；文字后期处理

## 新中式 / 国潮（New Chinese / Guochao）　★精选
- 主体占位符示例：[主体：如 中秋限定茶饮包装]
- 适配：通用；汉字生成易错，建议后期替换

**英文模板**
```
[subject], modern Chinese guochao style, traditional patterns reimagined, calligraphy accents, auspicious clouds, cinnabar red and indigo, contemporary layout, symmetrical or shan-shui inspired composition with negative space, soft warm light, cinnabar red, indigo, gold foil accents, ink black, rice paper beige
```
**中文模板**
```
[主体：如 中秋限定茶饮包装]，新中式国潮风格，传统纹样现代化，书法点缀，祥云，朱砂红与黛青，现代版式，对称或山水式留白构图，柔和暖光，朱砂红、黛青、金箔点缀、墨黑、宣纸米色
```
**负面词**：EN `cluttered symbols, garish red-gold, Japanese or Korean motifs, misspelled Chinese characters`｜中文 符号堆砌、俗艳红金、日韩元素混淆、错字

**Midjourney 示例**
```
[subject], modern Chinese guochao style, traditional patterns reimagined, calligraphy accents, auspicious clouds, cinnabar red and indigo, contemporary layout, symmetrical or shan-shui inspired composition with negative space, soft warm light, cinnabar red, indigo, gold foil accents, ink black, rice paper beige --ar 3:4 --no cluttered symbols, garish red-gold
```
**SD 写法**：Positive = 英文模板；Negative = `cluttered symbols, garish red-gold, Japanese or Korean motifs, misspelled Chinese characters, lowres, blurry, watermark`

- 应用建议：传统纹样需考据出处；避免与日式/韩式元素混淆

## 赛博朋克（Cyberpunk）
- 主体占位符示例：[主体：如 未来城市街景]
- 适配：MJ/SD 均擅长

**英文模板**
```
[subject], cyberpunk, neon-lit rainy street, holographic signage, high-tech low-life, reflective wet surfaces, low angle wide shot, neon rim light, volumetric fog, magenta, cyan, acid green on black
```
**中文模板**
```
[主体：如 未来城市街景]，赛博朋克，霓虹雨夜街道，全息招牌，高科技低生活，湿润反光地面，低机位广角，霓虹轮廓光、体积雾，黑底+品红、青、酸性绿
```
**负面词**：EN `daylight, pastel, clean minimal`｜中文 白天、粉彩、干净极简

**Midjourney 示例**
```
[subject], cyberpunk, neon-lit rainy street, holographic signage, high-tech low-life, reflective wet surfaces, low angle wide shot, neon rim light, volumetric fog, magenta, cyan, acid green on black --ar 3:4 --no daylight, pastel
```
**SD 写法**：Positive = 英文模板；Negative = `daylight, pastel, clean minimal, lowres, blurry, watermark`

- 应用建议：控制霓虹数量，留出主体

## 有机自然风（Organic / Biophilic）
- 主体占位符示例：[主体：如 有机护肤品产品图]
- 适配：通用

**英文模板**
```
[subject], organic natural style, earthy tones, soft curves, botanical elements, linen and clay textures, still life with natural props, soft morning sunlight with leaf shadows, sage green, terracotta, sand beige
```
**中文模板**
```
[主体：如 有机护肤品产品图]，有机自然风，大地色调，柔和曲线，植物元素，亚麻与陶土质感，带自然道具的静物，柔和晨光+树叶投影，鼠尾草绿、陶土色、沙米色
```
**负面词**：EN `neon, plastic, metallic, harsh light`｜中文 霓虹、塑料、金属、硬光

**Midjourney 示例**
```
[subject], organic natural style, earthy tones, soft curves, botanical elements, linen and clay textures, still life with natural props, soft morning sunlight with leaf shadows, sage green, terracotta, sand beige --ar 3:4 --no neon, plastic
```
**SD 写法**：Positive = 英文模板；Negative = `neon, plastic, metallic, harsh light, lowres, blurry, watermark`

- 应用建议：道具不宜过多，突出产品

## 酸性图形（Acid Graphics）
- 主体占位符示例：[主体：如 电子音乐节海报]
- 适配：MJ 风格化效果更佳

**英文模板**
```
[subject], acid graphics, liquid chrome, distorted experimental typography, star bursts, rave aesthetic, broken grid, centered chaos, high-contrast metallic reflections, black, silver, acid green
```
**中文模板**
```
[主体：如 电子音乐节海报]，酸性图形，液态铬金属，扭曲实验字体，星芒，锐舞美学，打破网格的居中构图，高对比金属反射，黑、银、酸性绿
```
**负面词**：EN `pastel, soft, corporate, photorealistic people`｜中文 粉彩、柔和、商务、写实人物

**Midjourney 示例**
```
[subject], acid graphics, liquid chrome, distorted experimental typography, star bursts, rave aesthetic, broken grid, centered chaos, high-contrast metallic reflections, black, silver, acid green --ar 3:4 --no pastel, soft
```
**SD 写法**：Positive = 英文模板；Negative = `pastel, soft, corporate, photorealistic people, lowres, blurry, watermark`

- 应用建议：主信息（时间地点）后期用可读字体排

## 奢华黑金（Luxury Black & Gold / Art Deco）
- 主体占位符示例：[主体：如 高端腕表海报]
- 适配：通用

**英文模板**
```
[subject], luxury black and gold, art deco ornaments, elegant serif typography, high contrast, premium, symmetrical centered composition, dramatic spotlight, deep black, champagne gold
```
**中文模板**
```
[主体：如 高端腕表海报]，奢华黑金，装饰艺术纹样，优雅衬线字体，高对比，高级感，对称居中构图，戏剧性聚光，深黑、香槟金
```
**负面词**：EN `cheap glitter, cluttered, bright colors`｜中文 廉价亮片、杂乱、高饱和

**Midjourney 示例**
```
[subject], luxury black and gold, art deco ornaments, elegant serif typography, high contrast, premium, symmetrical centered composition, dramatic spotlight, deep black, champagne gold --ar 3:4 --no cheap glitter, cluttered
```
**SD 写法**：Positive = 英文模板；Negative = `cheap glitter, cluttered, bright colors, lowres, blurry, watermark`

- 应用建议：金色控制在 10% 以内面积（经验值，推测）

## 电影感写实（Cinematic Realism）
- 主体占位符示例：[主体：如 一位站在雨中车站的女性]
- 适配：通用；MJ 可用 --ar 239:100 之类宽比

**英文模板**
```
[subject], cinematic still, anamorphic lens, film grain, shallow depth of field, color graded, wide 2.39:1 frame, rule of thirds, motivated practical lighting, backlight, teal and orange or muted desaturated
```
**中文模板**
```
[主体：如 一位站在雨中车站的女性]，电影剧照，变形宽银幕镜头，胶片颗粒，浅景深，电影调色，2.39:1 宽画幅，三分法，有动机的实景光源、逆光，青橙或低饱和
```
**负面词**：EN `oversaturated, flat lighting, cartoon`｜中文 过饱和、平光、卡通

**Midjourney 示例**
```
[subject], cinematic still, anamorphic lens, film grain, shallow depth of field, color graded, wide 2.39:1 frame, rule of thirds, motivated practical lighting, backlight, teal and orange or muted desaturated --ar 3:4 --no oversaturated, flat lighting
```
**SD 写法**：Positive = 英文模板；Negative = `oversaturated, flat lighting, cartoon, lowres, blurry, watermark`

- 应用建议：用 StudioBinder/EyeCannndy 术语描述镜头（low angle、dolly in）
