---
title: "网站资源总表"
description: "原文 100 个设计网站 + 15 个文章之外补充站点：内容、资源类型、作品风格、适用场景、推荐用途与逐站核验状态（表一）"
updated: 2026-11-26
tags: [sites, resources, verification, design-kb]
---

# 01 网站资源总表（表一）与网站内容定位（第一轮成果）

> 核验日期：2026-11-15（Asia/Shanghai）。方法：curl（桌面 UA）→ 失败则 WebFetch → 再用无头 Chrome 截图。各站点收录数量等简介信息整理自公开介绍。

**核验统计（文章 100 个）**：✅ 已核验 97｜🟡 部分核验 2｜❌ 访问失败 1　**扩展 15 个**：✅ 13｜🟡 1｜❌ 1

## 表一 网站资源总表

| # | 网站名称 | 链接 | 主要内容 | 资源类型 | 设计特点（收录作品风格） | 适用场景 | 推荐用途 | 信息核验情况 |
|---|---|---|---|---|---|---|---|---|
| 1 | Pwnisher 3D 渲染挑战赛 | https://www.youtube.com/@pwnisher | 同一白模/相机轨迹、全球数千人同题创作的3D渲染挑战赛合集 | 赛事/视频 | 写实与风格化3D并存，电影级打光、氛围叙事 | 3D打光、场景氛围对比学习 | 同题横向对比打光与创意 | ✅ 已核验：curl HTTP 200，页面标题「pwnisher - YouTube」 |
| 2 | Awwwards | https://www.awwwards.com/ | 每日最佳网站评选（设计/易用/创意/内容四项）+年度奖 | 奖项/网页灵感 | 超大字排版、沉浸式WebGL、滚动动效、深色高级感 | 网页趋势追踪、提案参考 | 每天5分钟刷趋势 | ✅ 已核验：curl HTTP 200，页面标题「Awwwards - Website Awards - Best Web Design Trends」 |
| 3 | CSS Design Awards | https://www.cssdesignawards.com/ | 每日最佳网站（UI/UX/创新三项评分） | 奖项/网页灵感 | 作品集站、实验交互、3D与动效 | 与 Awwwards 互补的网页选品 | 对比两家评委口味 | ✅ 已核验：curl 返回 202 空页（安全校验）；WebFetch 取得首页正文（当日 WOTD 列表） |
| 4 | The FWA | https://thefwa.com/ | 2000年起的数字设计奖，每日一个获奖项目 | 奖项/网页灵感 | 偏技术流：WebGL、声音互动、实验交互 | 找创意技术、互动营销案例 | 研究交互与技术表现 | ✅ 已核验：curl HTTP 200，页面标题「The FWA — Digital design awards since 2000」 |
| 5 | The Motion Awards | https://motionawards.com/ | Motionographer 主办的动态设计专项奖（片头/广告/品牌包装/AI单元） | 奖项/视频 | 片头、品牌动态、动态排版、AI影像 | 年度动态作品集中观摩 | 按单元刷年度最佳动态 | ✅ 已核验：curl HTTP 200（页面无 title 标签，正文可见）；无头浏览器截图正常 |
| 6 | Apple Design Awards | https://developer.apple.com/design/awards/ | 苹果WWDC年度App与游戏设计奖，附官方评语 | 奖项/UI | 果味UI、精致微交互、玻璃质感与拟物细节 | 移动端设计标杆 | 读评语理解'为什么好' | ✅ 已核验：curl HTTP 200，页面标题「Apple Design Awards - 2026 winners and finalists -」 |
| 7 | D&AD | https://www.dandad.org/ | 英国设计与广告大奖（黄铅笔/黑铅笔）及历年档案 | 奖项/品牌广告 | 品牌识别、广告创意、平面与工艺 | 品牌/广告/平面提案参考 | 翻历年获奖案例 | ✅ 已核验：curl HTTP 200，页面标题「D&AD」 |
| 8 | The One Show & ADC | https://www.oneclub.org/ | The One Club 两大奖：One Show 重创意，ADC 重视觉/字体/工艺 | 奖项/品牌广告 | 广告创意、字体排印、视觉工艺 | 广告创意与字体排印参考 | 区分创意奖与视觉奖 | ✅ 已核验：curl HTTP 200，页面标题「The One Show & ADC Awards ／ Advertising & Design A」 |
| 9 | Runway AI Film Festival | https://aif.runwayml.com/ | Runway 主办的AI影像节，Screening Room 可看历届获奖片 | 奖项/AI影像 | AI生成短片、超现实、实验影像 | 了解AI视频上限 | 看获奖片定AI视频目标 | ✅ 已核验：curl HTTP 200，页面标题「AIF 2026 ／ AI Festival」 |
| 10 | Tokyo TDC | https://tokyotypedirectorsclub.org/ | 东京字体指导俱乐部年度奖，亚洲视觉设计风向标 | 奖项/字体平面 | 实验字体、海报、书籍、动态视觉 | 实验字体/海报灵感 | 看实验性平面洗眼睛 | ✅ 已核验：curl HTTP 200，页面标题「Tokyo TDC」 |
| 11 | Annecy 安纳西国际动画节 | https://www.annecyfestival.com/ | 1960年创办的法国动画节，含商业委托单元 | 奖项/动画 | 多元动画美术风格、角色动画、MV/广告动画 | 动画美术与叙事参考 | 看商业委托单元 | ✅ 已核验：curl HTTP 200，页面标题「Site officiel du Festival et du Marché internation」 |
| 12 | Ciclope Festival | https://www.ciclopefestival.com/ | 按工种（导演/摄影/调色/剪辑/三维/配乐等）评奖的影视广告节 | 奖项/视频工艺 | 广告片的调色、剪辑、摄影工艺 | 单项工艺研究（调色/剪辑） | 按工种拆片 | ✅ 已核验：curl HTTP 200，页面标题「CICLOPE Festival」 |
| 13 | Motionographer | https://motionographer.com/ | 动态设计精选媒体+工作室幕后手记 | 媒体/动态 | 2D/3D动态、品牌动画、片头 | 动态作品拉片 | 每周固定刷新作 | ✅ 已核验：curl HTTP 200，页面标题「Motionographer®  Unexpected Inspiration™」 |
| 14 | STASH | https://www.stashmedia.tv/ | 按风格技法归档的动画/VFX/MV片库，附 Making-of（付费） | 片库/动态 | 商业广告、MV、频道包装、制作拆解 | 学习制作流程 | 看 Making-of | ✅ 已核验：curl HTTP 200，页面标题「Motion design - STASH - Welcome to the planet’s la」 |
| 15 | Art of the Title | https://www.artofthetitle.com/ | 电影/剧集/游戏片头设计研究+主创长访谈 | 媒体/片头 | 片头设计、动态排版、电影感 | 片头/开场设计 | 读主创访谈看草图分镜 | ✅ 已核验：curl HTTP 200，页面标题「Art of the Title」 |
| 16 | Vimeo Staff Picks | https://vimeo.com/channels/staffpicks | Vimeo 编辑每日人工精选短片 | 片库/短片 | 实拍短片、实验动画、纪录片 | 短片灵感 | 找稳定高水准短片 | ✅ 已核验：curl HTTP 200，页面标题「Vimeo Staff Picks on Vimeo」 |
| 17 | Behance 动态设计专区 | https://www.behance.net/galleries/motion | Behance Motion 分类：常附情绪板、风格帧、动态分镜与成片 | 作品集/动态 | 3D、插画动画、品牌动态等多元风格 | 学习完整交稿流程 | 看 Styleframe→成片 | ✅ 已核验：curl/WebFetch 403（反爬）；无头 Chrome 渲染出 Motion 分类页 |
| 18 | Short of the Week | https://www.shortoftheweek.com/ | 全球独立短片推荐+编辑影评 | 片库/短片 | 实拍与动画短片、叙事 | 叙事与短片学习 | 读影评学叙事 | ✅ 已核验：curl HTTP 200，页面标题「Short of the Week ／ The Best Short Films」 |
| 19 | Directors Notes | https://directorsnotes.com/ | 独立导演访谈博客（预算、器材、后期） | 媒体/访谈 | 独立短片、实拍 | 接片/拍摄实务参考 | 看器材与流程 | ✅ 已核验：curl HTTP 200，页面标题「Directors Notes // The Home of Independent Filmmak」 |
| 20 | Sakugabooru | https://www.sakugabooru.com/ | 动画作画片段库（原文称32万+条，带原画师/作品/类型标签） | 片段库/动画 | 日本动画作画、特效作画、角色表演 | 研究动作节奏与弹性 | 按标签逐帧看动作 | ✅ 已核验：curl HTTP 200，页面标题「sakugabooru」 |
| 21 | Promonews | https://www.promonews.tv/ | 每日精选MV与广告片+导演创作说明 | 媒体/MV | 风格化镜头、大胆调色、剪辑节奏 | 找视觉风格与调色参考 | 刷MV找风格 | ✅ 已核验：curl HTTP 200，页面标题「Music video creativity everyday ／ Promonews」 |
| 22 | BUCK | https://buck.co/ | 全球知名动态设计工作室作品集 | 工作室官网 | 2D/3D/实拍结合，插画动画，品牌片 | 大厂品牌动态参考 | 下载拉片逐帧拆 | ✅ 已核验：curl HTTP 200，页面标题「BUCK」 |
| 23 | ManvsMachine | https://mvsm.com/ | 伦敦创意工作室，三维材质与产品广告 | 工作室官网 | 3D材质碰撞、产品光影、硬核质感 | 产品广告/3D质感 | 研究材质与光影 | ✅ 已核验：curl HTTP 200，页面标题「ManvsMachine」 |
| 24 | Oddfellows | https://oddfellows.tv/ | 插画风与2D角色动画工作室（官网地址显示 Portland） | 工作室官网 | 插画、2D角色动画、品牌系统 | 插画动画与品牌动态 | 学配色与动作惯性 | ✅ 已核验：curl 首次 TLS 断开、重试 202；WebFetch 取得作品列表正文 |
| 25 | Golden Wolf | https://www.goldenwolf.tv/ | 伦敦动画工作室 | 工作室官网 | 高饱和撞色、夸张透视、快节奏街头卡通 | 年轻化/潮流动画 | 学高能量配色与节奏 | ✅ 已核验：curl HTTP 200，页面标题「Golden Wolf」 |
| 26 | Ordinary Folk | https://www.ordinaryfolk.co/ | 温哥华动态团队，2D几何图形动画 | 工作室官网 | 几何图形、弹性运动曲线 | 几何动态/信息动效 | 学运动曲线 | ✅ 已核验：curl HTTP 200，页面标题「Ordinary Folk – Motion Design & Animation Studio, 」 |
| 27 | ArtStation | https://www.artstation.com/ | CG/游戏美术作品社区 | 作品集/社区 | 概念设计、写实3D、奇幻/科幻 | CG/游戏美术参考 | 搜风格化概念设计 | ✅ 已核验：curl 403（Cloudflare challenge）、WebFetch 500；无头 Chrome 渲染出首页 |
| 28 | The Rookies | https://www.therookies.co/ | 面向学生与新人的年度比赛社区 | 社区/赛事 | 3D动画、游戏、VFX、概念设计 | 作品集对标 | 看应届作品水平 | ✅ 已核验：curl HTTP 200，页面标题「The Rookies - Creative Community for Next-Gen Arti」 |
| 29 | 80 Level | https://80.lv/ | 游戏美术与三维技术媒体，Breakdown 制作拆解 | 媒体/3D | 游戏场景、写实3D、技术美术 | 3D制作流程学习 | 读 Breakdown | ✅ 已核验：curl HTTP 200，页面标题「80 Level」 |
| 30 | Sketchfab | https://sketchfab.com/ | 网页3D模型查看与发布平台（可切线框/法线） | 平台/3D资产 | 各类3D模型、写实与低模 | 看布线与贴图通道 | 拆模型结构 | ✅ 已核验：curl HTTP 200，页面标题「Sketchfab - The best 3D viewer on the web」 |
| 31 | befores & afters | https://beforesandafters.com/ | 好莱坞视效幕后杂志 | 媒体/VFX | 视效前后对比、合成 | VFX流程学习 | 看前后对比 | ✅ 已核验：curl HTTP 200，页面标题「befores & afters - VFX magazine」 |
| 32 | fxguide | https://www.fxguide.com/ | 资深影视视效技术媒体 | 媒体/VFX | 渲染、虚拟制片、流体解算 | 技术美术进阶 | 读技术深文 | ✅ 已核验：curl HTTP 200，页面标题「fxguide」 |
| 33 | Blender Studio | https://studio.blender.org/ | Blender 官方开源动画工作室，教程与工程文件（付费） | 教程/资产 | 风格化3D动画短片 | Blender 学习 | 下载工程文件拆解 | ✅ 已核验：curl HTTP 200，页面标题「Blender Studio」 |
| 34 | Poly Haven | https://polyhaven.com/ | CC0 免费 HDRI、PBR 材质、扫描模型 | 素材/3D资产 | 写实材质、环境光 | 3D渲染素材 | 下载 HDRI/材质 | ✅ 已核验：curl HTTP 200，页面标题「Poly Haven」 |
| 35 | Beeple Everydays | https://beeple-crap.com/everydays | Beeple 自2007年起的每日一图（页面显示 7,137 天） | 作品集/数字艺术 | 超现实3D、赛博、讽刺 | 数字艺术/坚持练习 | 看长期练习轨迹 | ✅ 已核验：curl HTTP 200，页面标题「Everydays ／ BEEPLE」 |
| 36 | ShotDeck | https://shotdeck.com/ | 电影截图库，官网称150万+可检索镜头（付费） | 截图库/影视 | 电影级布光、构图、调色 | 电影感布光/构图参考 | 按光线/镜头/色调筛 | ✅ 已核验：curl 403（Cloudflare）；WebFetch 取得首页正文 |
| 37 | FILMGRAB | https://film-grab.com/ | 免费电影截图站，一片一页 | 截图库/影视 | 经典电影关键帧 | 研究导演用光构图 | 整片关键帧对比 | ✅ 已核验：curl HTTP 200，页面标题「[FILMGRAB]」 |
| 38 | StillsLab | https://stillslab.com/ | 免费影视截图库，细标签+统计（如夜景占比） | 截图库/影视 | 电影/剧集/MV/广告画面 | 视觉配方研究 | 按景别/光线筛选 | ✅ 已核验：curl HTTP 200，页面标题「StillsLab — Movie Stills & TV Show Frames for Film」 |
| 39 | Flim | https://flim.ai/ | AI 语义搜索影视截图 | 截图库/AI搜索 | 电影、MV、广告画面 | 用自然语言找镜头 | 描述画面搜索 | ✅ 已核验：curl HTTP 200，页面标题「Flim ／ AI search engine for film stills and visual」 |
| 40 | EyeCannndy | https://eyecannndy.com/ | 镜头语言与剪辑技法动图词典 | 词典/影视 | 转场、运镜、剪辑技法实例 | 给技法命名、写AI视频提示词 | 查技法名称 | ✅ 已核验：curl HTTP 200，页面标题「Eyecandy - Visual Technique Library」 |
| 41 | StudioBinder 镜头语言指南 | https://www.studiobinder.com/blog/ultimate-guide-to-camera-shots/ | 景别/机位/运镜系统教程 | 教程/影视 | 电影实例配图 | AI视频提示词术语 | 查 low angle、dolly in 等 | ✅ 已核验：curl HTTP 200，页面标题「50+ Types of Camera Shots, Angles, and Techniques」 |
| 42 | American Cinematographer（ASC） | https://theasc.com/ | 美国电影摄影师协会杂志与站点 | 媒体/摄影 | 摄影指导讲解镜头与布光 | 理解'为什么这么拍' | 读摄影指导文章 | 🟡 部分核验：curl 与无头浏览器均返回 Cloudflare 520；WebFetch 取得新闻标题（站点间歇性故障） |
| 43 | Mobbin | https://mobbin.com/ | 真实App截图库（原文称60万+界面，付费，免费号可看部分） | 截图库/UI | 主流App的扁平/极简界面与流程 | 功能页对标（订阅页、空状态等） | 按功能标签筛 | ✅ 已核验：curl HTTP 200，页面标题「Mobbin — UI & UX design inspiration for mobile & w」 |
| 44 | Page Flows | https://pageflows.com/ | 真实产品操作录屏（付费） | 录屏库/UX | 完整用户流程 | 交互流程梳理 | 看注册/付费/取消流程 | ✅ 已核验：curl HTTP 200，页面标题「UI/UX Design Inspiration & User Flows from Top App」 |
| 45 | Refero | https://refero.design/ | Web/iOS界面截图库，标签细（付费）；子站 styles.refero.design | 截图库/UI | SaaS与消费级Web界面 | 组件/页面类型检索 | 搜具体组件 | ✅ 已核验：curl HTTP 200，页面标题「Refero — UI/UX Design Inspiration for Your Next Pr」 |
| 46 | Nicelydone | https://nicelydone.club/ | SaaS/Web应用界面库（付费） | 截图库/UI | ToB后台、表单、数据看板 | B端设计参考 | 找复杂表单/看板 | ✅ 已核验：curl HTTP 200，页面标题「Nicelydone — Web apps design inspiration (UX & UI)」 |
| 47 | SaaSFrame | https://www.saasframe.io/ | SaaS产品界面库（付费） | 截图库/UI | 营销页、登录、设置页 | 独立开发/B端 | 按页面类型翻 | ✅ 已核验：curl HTTP 200，页面标题「SaaSFrame - SaaS UI & UX Design Inspiration Librar」 |
| 48 | Figma Community | https://www.figma.com/community | Figma 开源社区：模板、插件、设计系统源文件 | 社区/源文件 | 设计系统、UI Kit、模板 | 直接拆源文件 | 学 Auto Layout 与变量 | ✅ 已核验：curl HTTP 200，页面标题「Discover community-made templates, plugins, and wi」 |
| 49 | Apple 人机界面指南（HIG） | https://developer.apple.com/design/human-interface-guidelines/ | 苹果官方设计规范 | 规范文档 | 苹果平台交互与视觉规范（含材质/玻璃效果） | iOS/macOS 设计依据 | 查规范 | ✅ 已核验：curl HTTP 200，页面标题「Human Interface Guidelines ／ Apple Developer Docum」 |
| 50 | Material Design 3 | https://m3.material.io/ | Google 设计系统文档 | 规范文档 | 色阶、字号层级、动态配色、组件状态 | 设计系统搭建 | 学色阶与状态逻辑 | ✅ 已核验：curl HTTP 200，页面标题「Material Design」 |
| 51 | Vercel Web Interface Guidelines | https://vercel.com/design/guidelines | 界面细节检查清单（交互/动画/布局/文案/表单/性能） | 规范清单 | 克制、细节导向的现代Web | 上线前自查 | 逐条检查 | ✅ 已核验：curl HTTP 200，页面标题「Web Interface Guidelines」 |
| 52 | Impeccable | https://impeccable.style/ | 面向AI编码代理的'去AI味'设计 skill（原文称62项检查） | AI设计工具 | 反模板化、去'AI味' | 约束AI生成UI | 让Agent自查 | ✅ 已核验：curl HTTP 200，页面标题「Impeccable: The missing design vocabulary for agen」 |
| 53 | The Component Gallery | https://component.gallery/ | 跨设计系统组件对比（首页称60组件/95设计系统/2,671示例） | 组件库索引 | 各大设计系统组件 | 组件设计对标 | 同一组件多家对比 | ✅ 已核验：curl HTTP 200，页面标题「The Component Gallery」 |
| 54 | 60fps | https://60fps.design/ | 高帧率UI动效片段库 | 动效库/UI | 卡片展开、下拉刷新、页面过渡 | 微交互灵感 | 找动效手感 | ✅ 已核验：curl HTTP 200，页面标题「60fps - UI/UX animation inspiration for mobile & w」 |
| 55 | Spotted in Prod | https://www.spottedinprod.com/ | 已上线iOS应用的细节短视频 | 动效库/UI | 微交互、彩蛋、触感反馈可视化 | 细节打磨 | 抠细节 | ✅ 已核验：curl HTTP 200，页面标题「Spotted in Prod — The very best of iOS」 |
| 56 | Growth.Design | https://growth.design/ | 连环画形式拆解知名App体验 | 案例/UX | 用户心理与转化 | 增长与转化设计 | 读案例学文案与心理 | ✅ 已核验：curl HTTP 200，页面标题「Growth.Design — Better Products, Better Growth.」 |
| 57 | Laws of UX | https://lawsofux.com/ | UX心理学定律卡片 | 知识卡片/UX | 菲茨/希克/米勒等定律 | 写方案找依据 | 查定律 | ✅ 已核验：curl HTTP 200，页面标题「Home ／ Laws of UX」 |
| 58 | Game UI Database | https://www.gameuidatabase.com/ | 游戏UI截图库（首页显示 1,997 款游戏/79,623 张截图） | 截图库/游戏UI | HUD、背包、技能树等 | 游戏UI参考 | 按功能搜界面 | ✅ 已核验：curl HTTP 200，页面标题「Game UI Database 2.0 ／ Welcome」 |
| 59 | Recent（原 Godly） | https://recent.design/ | 网页灵感库，缩略图即播滚动录屏（godly.website 301 跳转至此） | 网页灵感 | 深色、WebGL、实验动效、大字 | 前沿网页灵感 | 看滚动录屏 | ✅ 已核验：curl HTTP 200，页面标题「Recent — Design Inspiration」 |
| 60 | Siteinspire | https://www.siteinspire.com/ | 老牌网页灵感库，风格/类型/行业叠加筛选 | 网页灵感 | 极简、网格、非常规版式、艺术摄影类网站 | 克制型网页参考 | 按风格+行业筛 | ✅ 已核验：curl 429（Vercel Security Checkpoint）；WebFetch 取得作品列表 |
| 61 | Land-book | https://land-book.com/ | 落地页图库（含定价页/关于页/简历页） | 网页灵感/落地页 | SaaS落地页、渐变、卡片 | 商业网站 | 按页面类型找 | ✅ 已核验：curl HTTP 200，页面标题「Landbook - website design inspiration gallery」 |
| 62 | Landingfolio | https://www.landingfolio.com/ | 落地页+区块拆解（原文称4600+区块，部分付费） | 网页灵感/区块 | 首屏、功能、评价、CTA 区块 | 区块级参考、喂AI | 复制区块结构 | ✅ 已核验：curl HTTP 200，页面标题「The Best Landing Page Design Inspiration, Template」 |
| 63 | awesome-design-md | https://github.com/VoltAgent/awesome-design-md | GitHub 开源合集：知名品牌网站的 DESIGN.md | AI设计规范 | Stripe/Linear/Vercel/Apple 等品牌风格 | 让AI按品牌风格生成UI | 放入项目约束AI | ✅ 已核验：curl HTTP 200，页面标题「GitHub - VoltAgent/awesome-design-md: A collection」 |
| 64 | One Page Love | https://onepagelove.com/ | 单页网站合集与模板 | 网页灵感 | 单页叙事、活动页、个人页 | 单页/活动页 | 学单页节奏 | ✅ 已核验：curl HTTP 200，页面标题「One Page Love — One Page Website Inspiration and T」 |
| 65 | Minimal Gallery | https://minimal.gallery/ | 极简风格网站图库 | 网页灵感 | 黑白灰、大留白、字号对比 | 极简网页 | 学留白与层级 | ✅ 已核验：curl HTTP 200，页面标题「Minimal Gallery – Hand-picked web design inspirati」 |
| 66 | Dark Mode Design | https://www.darkmodedesign.com/ | 只收深色模式网页 | 网页灵感 | 深色层级、细线边框、微光 | 深色界面 | 学深色层级 | ✅ 已核验：curl HTTP 200，页面标题「Dark Mode Design 🌘 Handpicked website inspiration」 |
| 67 | Hoverstat.es | https://www.hoverstat.es/ | 另类/实验网页合集 | 网页灵感 | 非常规导航、实验交互、反商业 | 找反套路灵感 | 看实验网页 | ✅ 已核验：curl HTTP 200，页面标题「HOVERSTAT.ES ／ The home of alternative web-design.」 |
| 68 | Web Design Museum | https://www.webdesignmuseum.org/ | 1991–2006 网页设计历史档案 | 档案/网页史 | 早期门户、拟物按钮、Flash | 复古网页/Y2K 参考 | 查年代视觉 | ✅ 已核验：curl HTTP 200，页面标题「Web Design Museum – Discover old websites, apps, s」 |
| 69 | Codrops | https://tympanus.net/codrops/ | 创意前端教程与 Demo | 教程/前端 | WebGL扭曲、页面过渡、滚动文字 | 创意前端实现 | 照教程复现 | ✅ 已核验：curl HTTP 200，页面标题「Codrops ／ Fueling web creativity since 2009」 |
| 70 | CodePen Spark | https://codepen.io/spark | CodePen 每周创意代码精选 | 代码合集/前端 | CSS/SVG/Canvas/Three.js 小作品 | 找前端小特效 | 改参数学原理 | ✅ 已核验：curl 403（Cloudflare）；WebFetch 取得本周 Spark 列表 |
| 71 | GSAP 官方 Demo 库 | https://demos.gsap.com/ | GSAP 动画示例（滚动/文字/悬停等） | 示例库/前端动画 | 滚动叙事、文字动画 | 网页动效实现 | 复制 CodePen 源码 | ✅ 已核验：curl HTTP 200，页面标题「GSAP Demo Hub」 |
| 72 | Three.js 官方示例 | https://threejs.org/examples/ | Three.js 数百个官方 Demo | 示例库/WebGL | 3D渲染、物理、后期 | Web3D 入门与查效果 | 查示例源码 | ✅ 已核验：curl HTTP 200，页面标题「three.js examples」 |
| 73 | Shadertoy | https://www.shadertoy.com/ | GLSL 着色器作品社区 | 社区/图形学 | 程序化生成画面、体积云、霓虹城市 | 着色器灵感 | 看 shader 源码 | 🟡 部分核验：curl 403、无头浏览器遇安全校验；WebFetch 仅得标题'Shader of the Week' |
| 74 | The Book of Shaders | https://thebookofshaders.com/ | 片元着色器互动教程（含中文版） | 教程/图形学 | 程序化图形、噪波 | 学 shader 基础 | 跟教程练习 | ✅ 已核验：curl HTTP 200，页面标题「The Book of Shaders」 |
| 75 | Bruno Simon | https://bruno-simon.com/ | 可驾驶玩具车的3D作品集 | 个人站/WebGL | 游戏化3D交互 | 创意作品集 | 体验游戏化交互 | ✅ 已核验：curl HTTP 200，页面标题「Bruno's」 |
| 76 | Lusion | https://lusion.co/ | 英国WebGL创意开发工作室 | 工作室官网 | 3D粒子转场、滚轮阻尼、音效 | 高端互动网页 | 观摩交互细节 | ✅ 已核验：curl HTTP 200，页面标题「Lusion - Award Winning 3D and Interactive Web Stud」 |
| 77 | Active Theory | https://activetheory.net/ | 美国数字互动工作室 | 工作室官网 | 大型互动营销、3D粒子 | 互动营销案例 | 看项目案例 | ✅ 已核验：curl HTTP 200，页面标题「Active Theory · Creative Digital Experiences」 |
| 78 | Framer Gallery | https://www.framer.com/gallery/ | Framer 搭建的优秀网站合集 | 网页灵感/建站 | 现代SaaS/作品集站、动效 | 无代码建站参考 | 找可复刻模板 | ✅ 已核验：curl HTTP 200，页面标题「Framer Gallery: Explore the best websites built wi」 |
| 79 | Motion 官方示例 | https://motion.dev/examples | Motion（原 Framer Motion）动画示例（部分付费） | 示例库/前端动画 | 弹簧缓动、列表重排、滚动动画 | React/Vue 动效实现 | 复制示例 | ✅ 已核验：curl HTTP 200，页面标题「Examples: React, JavaScript, and Vue animation sni」 |
| 80 | React Bits | https://reactbits.dev/ | 免费开源 React 动画组件 | 组件库/前端 | 文字乱码、磁吸按钮、流光边框、流体背景 | 快速加动效 | 复制组件 | ✅ 已核验：curl HTTP 200，页面标题「React Bits — Free Animated React Components」 |
| 81 | coss ui | https://coss.com/ui | Cal.com 设计系统（前身 Origin UI），Tailwind，MIT | 组件库/前端 | 克制、产品级组件 | 产品级组件 | 直接用组件 | ✅ 已核验：curl HTTP 200，页面标题「A modern React UI component library – coss ui」 |
| 82 | Josh W. Comeau | https://www.joshwcomeau.com/ | 交互式前端博客（CSS/动画/SVG） | 博客/教程 | 可交互图解 | CSS/动画原理 | 拖滑块理解原理 | ✅ 已核验：curl HTTP 200，页面标题「Josh W. Comeau」 |
| 83 | Rauno Freiberg | https://rauno.me/ | Vercel 设计工程师个人站，《Invisible Details of Interaction Design》 | 个人站/交互 | 交互细节 | 交互细节学习 | 读交互细节文章 | ✅ 已核验：curl HTTP 200，页面标题「Rauno Freiberg」 |
| 84 | Emil Kowalski | https://emilkowal.ski/ | Sonner/Vaul 作者博客，界面动画 | 博客/动效 | 克制跟手的动画 | 动画时长/缓动调校 | 读动画文章 | ✅ 已核验：curl HTTP 200，页面标题「Emil Kowalski」 |
| 85 | Typewolf | https://www.typewolf.com/ | 字体指南与真实网站字体搭配 | 字体指南 | 优秀网站字体搭配 | 选字体搭配 | 查字体组合 | ✅ 已核验：curl HTTP 200，页面标题「What’s Trending in Type  · Typewolf」 |
| 86 | Fonts In Use | https://fontsinuse.com/ | 真实世界字体使用档案 | 字体档案 | 海报、书封、唱片、网页 | 看字体实际效果 | 按字体检索案例 | ✅ 已核验：curl HTTP 200，页面标题「Fonts In Use - Fonts In Use」 |
| 87 | Google Fonts | https://fonts.google.com/ | 免费开源字库（含思源黑/宋等） | 字体库 | 开源字体 | 免费可商用字体 | 选字下载 | ✅ 已核验：curl HTTP 200，页面标题「Browse Fonts - Google Fonts」 |
| 88 | Fontshare | https://www.fontshare.com/ | ITF 免费字库（个人与商用免费） | 字体库 | 几何无衬线等精品字体 | 免费精品字体 | 选几何无衬线 | ✅ 已核验：curl HTTP 200（gzip 正文）；无头截图正常 |
| 89 | Butterick's Practical Typography | https://practicaltypography.com/ | 免费在线排版书 | 教程/排版 | 排版硬规则 | 排版基础 | 读'10分钟'章节 | ✅ 已核验：curl HTTP 200，页面标题「Butterick’s Practical Typography」 |
| 90 | Utopia | https://utopia.fyi/ | 流体字号/间距比例计算器 | 工具/排版 | 模块化字号比例 | 建立字号系统 | 生成 CSS 变量 | ✅ 已核验：curl HTTP 200，页面标题「Fluid Responsive Design ／ Utopia」 |
| 91 | Coolors | https://coolors.co/ | 配色生成器（空格随机、锁色、色盲模拟） | 工具/配色 | 五色卡 | 快速配色 | 生成并导出色卡 | ✅ 已核验：curl HTTP 200，页面标题「Coolors - The super fast color palettes generator!」 |
| 92 | Realtime Colors | https://www.realtimecolors.com/ | 在真实页面上实时预览配色（原文描述） | 工具/配色 | 文字/背景/主色/强调色预览 | 配色落地预览（当前不可用） | 暂用 Coolors+Radix 替代 | ❌ 访问失败：HTTP 402 DEPLOYMENT_DISABLED，页面显示'This deployment is temporarily paused'（站点部署被暂停，非网络问题） |
| 93 | Radix Colors | https://www.radix-ui.com/colors | 12级界面色阶系统 | 工具/配色 | 功能化色阶（背景/边框/文字） | 设计系统配色 | 按级取色 | ✅ 已核验：curl HTTP 200，页面标题「Radix Colors」 |
| 94 | tweakcn | https://tweakcn.com/ | shadcn/ui 可视化主题编辑器 | 工具/主题 | 换皮 shadcn 组件 | 避免 shadcn 同质化 | 调主题导出 | ✅ 已核验：curl HTTP 200，页面标题「Beautiful themes for shadcn/ui — tweakcn ／ Theme E」 |
| 95 | Pinterest | https://www.pinterest.com/ | 全网最大图片灵感平台 | 灵感收集 | 全风格（混杂） | 情绪板、顺藤摸瓜找同风格 | 相似图扩展 | ✅ 已核验：curl HTTP 200，页面标题「Pinterest」 |
| 96 | Are.na | https://www.are.na/ | 无算法、无点赞的研究型收集工具 | 灵感收集 | 研究资料、艺术、建筑 | 课题研究攒资料 | 建频道串联 | ✅ 已核验：curl HTTP 200，页面标题「Are.na」 |
| 97 | Cosmos | https://www.cosmos.so/ | 新一代灵感收藏夹（浏览器插件） | 灵感收集 | 高审美创意人公开收藏 | 收集好图视频 | 逛 Discover | ✅ 已核验：curl HTTP 200，页面标题「Cosmos」 |
| 98 | Savee | https://savee.com/ | 极简图片灵感社区 | 灵感收集 | 平面排版、品牌包装、先锋摄影、字体 | 高级感平面参考 | 刷瀑布流 | ✅ 已核验：curl HTTP 200，页面标题「Savee」 |
| 99 | It's Nice That | https://www.itsnicethat.com/ | 伦敦创意文化媒体 | 媒体/创意 | 插画、平面、动画、摄影 | 创意文化阅读 | 午间阅读 | ✅ 已核验：curl HTTP 200，页面标题「It's Nice That」 |
| 100 | Brand New | https://www.underconsideration.com/brandnew/ | 品牌换标点评（付费，免费可见新旧 Logo 对比） | 媒体/品牌 | 品牌识别系统演变 | 品牌设计判断力 | 看新旧对比 | ✅ 已核验：curl HTTP 200，页面标题「Brand New」 |

## 按原文九大类的详细条目（内容定位 + 原文要点）

### 一、大赛与奖项（12 个）

**1. Pwnisher 3D 渲染挑战赛** — https://www.youtube.com/@pwnisher
- 定位/资源类型：赛事/视频；领域标签：3D、视频
- 主要内容：同一白模/相机轨迹、全球数千人同题创作的3D渲染挑战赛合集
- 原文要点（摘录）：油管博主 Clinton Jones（网名 Pwnisher）办的全球 3D 渲染比赛。玩法特别直观：他给一段定死相机轨迹和人物动作的白模，全世界几千个参赛者在这个底子上各自发挥，最后拼成一支长视频。到 2026 年已经办了 13 届。因为所有人的底子完全一样，谁的打光好、谁的脑洞大，放一起对比看得清清楚楚。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：3D打光、场景氛围对比学习；同题横向对比打光与创意
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「pwnisher - YouTube」

**2. Awwwards** — https://www.awwwards.com/
- 定位/资源类型：奖项/网页灵感；领域标签：网页、前端
- 主要内容：每日最佳网站评选（设计/易用/创意/内容四项）+年度奖
- 原文要点（摘录）：做网页和前端绕不开的奖。每天评出一个「今日最佳网站」，评委按设计、易用性、创意、内容四项打分，年底还会选年度大奖。很适合每天早上开工前花五分钟刷一下，看看现在的网页设计又卷出了什么新花样。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：网页趋势追踪、提案参考；每天5分钟刷趋势
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Awwwards - Website Awards - Best Web Design Trends」

**3. CSS Design Awards** — https://www.cssdesignawards.com/
- 定位/资源类型：奖项/网页灵感；领域标签：网页、前端
- 主要内容：每日最佳网站（UI/UX/创新三项评分）
- 原文要点（摘录）：和 Awwwards 齐名的另一个网页大奖，也是每天推一个最佳站点，按 UI、UX、创新打分。它和 Awwwards 的评委口味不太一样，两边选出来的网站经常不重样，可以换着看。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：与 Awwwards 互补的网页选品；对比两家评委口味
- 核验：✅ 已核验（2026-11-15）curl 返回 202 空页（安全校验）；WebFetch 取得首页正文（当日 WOTD 列表）

**4. The FWA** — https://thefwa.com/
- 定位/资源类型：奖项/网页灵感；领域标签：网页、互动
- 主要内容：2000年起的数字设计奖，每日一个获奖项目
- 原文要点（摘录）：2000 年就开始办的老牌数字设计奖，也是每天更新一个获奖项目。相比规规矩矩的商业排版，FWA 更喜欢选那些在交互、WebGL、声音互动上玩出花来的技术流作品。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：找创意技术、互动营销案例；研究交互与技术表现
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「The FWA — Digital design awards since 2000」

**5. The Motion Awards** — https://motionawards.com/
- 定位/资源类型：奖项/视频；领域标签：动态、视频
- 主要内容：Motionographer 主办的动态设计专项奖（片头/广告/品牌包装/AI单元）
- 原文要点（摘录）：Motionographer 自己办的动态设计专项奖。片头、广告、品牌包装、纪录片各评各的，这两年还加了 AI 单元。最实在的是获奖页直接嵌着成片，不用再跳出去到处找，像《幕府将军》的片头就在里面，一个下午就能把一整年最好的动态作品刷一遍。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：年度动态作品集中观摩；按单元刷年度最佳动态
- 核验：✅ 已核验（2026-11-15）curl HTTP 200（页面无 title 标签，正文可见）；无头浏览器截图正常

**6. Apple Design Awards** — https://developer.apple.com/design/awards/
- 定位/资源类型：奖项/UI；领域标签：UI、移动端
- 主要内容：苹果WWDC年度App与游戏设计奖，附官方评语
- 原文要点（摘录）：苹果每年 WWDC 开发者大会上颁的奖。能上榜的 App 和游戏，在果味审美、交互手感和硬件特性结合上基本都是教科书级别的。苹果官方还会给每个获奖应用写一段评语，讲清楚为什么选它，做移动端的人非常值得细看。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：移动端设计标杆；读评语理解'为什么好'
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Apple Design Awards - 2026 winners and finalists -」

**7. D&AD** — https://www.dandad.org/
- 定位/资源类型：奖项/品牌广告；领域标签：品牌、广告、平面
- 主要内容：英国设计与广告大奖（黄铅笔/黑铅笔）及历年档案
- 原文要点（摘录）：英国的设计与广告大奖，因为奖杯造型是铅笔，国内同行一般叫它「黄铅笔奖」。它最高级别的「黑铅笔」评选极其苛刻，有些年份宁可空缺也不发，能拿下的全是能写进设计史的案子。做品牌、广告和平面的人可以多翻它的历年档案。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：品牌/广告/平面提案参考；翻历年获奖案例
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「D&AD」

**8. The One Show & ADC** — https://www.oneclub.org/
- 定位/资源类型：奖项/品牌广告；领域标签：品牌、广告、字体
- 主要内容：The One Club 两大奖：One Show 重创意，ADC 重视觉/字体/工艺
- 原文要点（摘录）：美国 The One Club 办的两个顶级大奖。One Show 更看重广告片背后的创意点子，而 1921 年创办的 ADC（纽约艺术指导俱乐部奖）更看重纯正的视觉表现、字体排印和工艺细节。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：广告创意与字体排印参考；区分创意奖与视觉奖
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「The One Show & ADC Awards ／ Advertising & Design A」

**9. Runway AI Film Festival** — https://aif.runwayml.com/
- 定位/资源类型：奖项/AI影像；领域标签：AI、视频
- 主要内容：Runway 主办的AI影像节，Screening Room 可看历届获奖片
- 原文要点（摘录）：AI 视频工具 Runway 办的 AI 影像节，2026 年已经是第 4 届，在纽约、洛杉矶、东京都有线下放映。除了短片，还分了设计、新媒体、时尚、广告几个赛道。官网的 Screening Room 能直接看历届获奖片，想知道 AI 视频的天花板现在到了哪儿，看这里最直接。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：了解AI视频上限；看获奖片定AI视频目标
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「AIF 2026 ／ AI Festival」

**10. Tokyo TDC** — https://tokyotypedirectorsclub.org/
- 定位/资源类型：奖项/字体平面；领域标签：字体、平面
- 主要内容：东京字体指导俱乐部年度奖，亚洲视觉设计风向标
- 原文要点（摘录）：东京字体指导俱乐部的年度奖。虽然名字里带「字体」，但它其实是整个亚洲视觉设计圈的风向标。评委眼光非常刁钻，获奖的海报、书籍和动态视觉大多带有很强的实验性，看腻了四平八稳的商业稿，去这儿洗洗眼睛特别好。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：实验字体/海报灵感；看实验性平面洗眼睛
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Tokyo TDC」

**11. Annecy 安纳西国际动画节** — https://www.annecyfestival.com/
- 定位/资源类型：奖项/动画；领域标签：动画、视频
- 主要内容：1960年创办的法国动画节，含商业委托单元
- 原文要点（摘录）：1960 年创办的法国动画节，动画人眼里的最高殿堂。除了动画长片和独立短片，它还有专门的商业委托单元（广告、MV、片头），能看到全世界最好的一批美术风格和动态叙事。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：动画美术与叙事参考；看商业委托单元
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Site officiel du Festival et du Marché internation」

**12. Ciclope Festival** — https://www.ciclopefestival.com/
- 定位/资源类型：奖项/视频工艺；领域标签：视频、广告
- 主要内容：按工种（导演/摄影/调色/剪辑/三维/配乐等）评奖的影视广告节
- 原文要点（摘录）：一个专门按「工种」发奖的影视广告节。别的奖大多看整体创意，它偏偏把片子拆开：导演、摄影、调色、剪辑、三维动画、视觉特效、配乐各评各的奖。做视频的人如果想单拎出「调色」或「剪辑节奏」来研究，看这个奖最对路。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：单项工艺研究（调色/剪辑）；按工种拆片
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「CICLOPE Festival」

### 二、动态设计与视频（14 个）

**13. Motionographer** — https://motionographer.com/
- 定位/资源类型：媒体/动态；领域标签：动态
- 主要内容：动态设计精选媒体+工作室幕后手记
- 原文要点（摘录）：动态设计圈办了快二十年的老牌网站。编辑挑片子的眼光很毒，平时不乱发水文，一旦更新基本都是值得反复拉片的好作品，还经常顺带放出工作室写的幕后制作手记。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：动态作品拉片；每周固定刷新作
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Motionographer®  Unexpected Inspiration™」

**14. STASH** — https://www.stashmedia.tv/
- 定位/资源类型：片库/动态；领域标签：动态、VFX
- 主要内容：按风格技法归档的动画/VFX/MV片库，附 Making-of（付费）
- 原文要点（摘录）：很多动画和视效工作室都会订的在线片库（付费）。里面按风格和技法归档了成千上万支商业广告、MV 和频道包装，最大的价值是很多片子附带了制作花絮（Making-of）和工程拆解。
- 价格：付费/部分付费
- 使用场景与价值：学习制作流程；看 Making-of
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Motion design - STASH - Welcome to the planet’s la」

**15. Art of the Title** — https://www.artofthetitle.com/
- 定位/资源类型：媒体/片头；领域标签：动态、影视
- 主要内容：电影/剧集/游戏片头设计研究+主创长访谈
- 原文要点（摘录）：专门研究电影、剧集和游戏「片头设计」的网站。它不光放高清片头视频，最下功夫的是长篇主创专访——把导演和设计师请来，把最初的草图、废稿、分镜脚本全摆出来，一步步讲这短短两分钟的片头是怎么磨出来的。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：片头/开场设计；读主创访谈看草图分镜
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Art of the Title」

**16. Vimeo Staff Picks** — https://vimeo.com/channels/staffpicks
- 定位/资源类型：片库/短片；领域标签：视频
- 主要内容：Vimeo 编辑每日人工精选短片
- 原文要点（摘录）：Vimeo 编辑部每天人工挑出来的短片频道。在视频圈子里，自己的作品能挂上一枚 Staff Pick 的标志是挺值得吹一辈子的事。不管是实拍短片、实验动画还是纪录片，水准都非常稳。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：短片灵感；找稳定高水准短片
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Vimeo Staff Picks on Vimeo」

**17. Behance 动态设计专区** — https://www.behance.net/galleries/motion
- 定位/资源类型：作品集/动态；领域标签：动态、品牌
- 主要内容：Behance Motion 分类：常附情绪板、风格帧、动态分镜与成片
- 原文要点（摘录）：虽然大家平时都在刷 Behance，但它的 Motion 分类尤其适合拿来学工作流。因为很多工作室在上面发项目时，会把前期的情绪板、风格帧（Styleframes）、动态分镜（Animatic）和最终成片一块儿放出来，相当于把整个交稿过程摊开给你看。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：学习完整交稿流程；看 Styleframe→成片
- 核验：✅ 已核验（2026-11-15）curl/WebFetch 403（反爬）；无头 Chrome 渲染出 Motion 分类页

**18. Short of the Week** — https://www.shortoftheweek.com/
- 定位/资源类型：片库/短片；领域标签：视频
- 主要内容：全球独立短片推荐+编辑影评
- 原文要点（摘录）：专门推荐全球优秀独立短片的网站，实拍和动画都有。每部片子下面都配了一篇编辑写的正经影评，帮你拆解导演是怎么在十几分钟里立住人物、讲完一个好故事的。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：叙事与短片学习；读影评学叙事
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Short of the Week ／ The Best Short Films」

**19. Directors Notes** — https://directorsnotes.com/
- 定位/资源类型：媒体/访谈；领域标签：视频
- 主要内容：独立导演访谈博客（预算、器材、后期）
- 原文要点（摘录）：一个做独立导演访谈的博客。每次聊一部短片，问的问题都很实在：当时怎么凑的钱、现场用的什么机器和镜头、后期遇到了什么麻烦。自己平时接片子、拍东西的人看这个会很有共鸣。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：接片/拍摄实务参考；看器材与流程
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Directors Notes // The Home of Independent Filmmak」

**20. Sakugabooru** — https://www.sakugabooru.com/
- 定位/资源类型：片段库/动画；领域标签：动画
- 主要内容：动画作画片段库（原文称32万+条，带原画师/作品/类型标签）
- 原文要点（摘录）：动画迷自己维护的「作画」片段库，存了 32 万多条从动画里剪出来的高光片段。每条都打好了标签：哪位原画师画的、出自哪部作品、是爆炸特效还是角色表演。想研究一个动作的节奏和弹性，搜标签就能拉出几百个片段逐帧看，做动画的人和用 AI 生成动作镜头的人都用得上。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：研究动作节奏与弹性；按标签逐帧看动作
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「sakugabooru」

**21. Promonews** — https://www.promonews.tv/
- 定位/资源类型：媒体/MV；领域标签：视频、MV
- 主要内容：每日精选MV与广告片+导演创作说明
- 原文要点（摘录）：每天精选几支新出的 MV 和广告片，大多配着导演的创作说明：用什么机器拍的、为什么这么调色、某个镜头是怎么做出来的。MV 是风格化镜头、色彩和剪辑节奏最敢玩的地方，想找视觉风格参考，刷这里比在视频网站上大海捞针高效得多。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：找视觉风格与调色参考；刷MV找风格
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Music video creativity everyday ／ Promonews」

**22. BUCK** — https://buck.co/
- 定位/资源类型：工作室官网；领域标签：动态、品牌
- 主要内容：全球知名动态设计工作室作品集
- 原文要点（摘录）：全球规模和名气最大的动态设计工作室之一，苹果、耐克、Meta 的常客。2D、3D、实拍结合全能，作品集大得像个博物馆。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：大厂品牌动态参考；下载拉片逐帧拆
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「BUCK」

**23. ManvsMachine** — https://mvsm.com/
- 定位/资源类型：工作室官网；领域标签：3D、广告
- 主要内容：伦敦创意工作室，三维材质与产品广告
- 原文要点（摘录）：伦敦的顶尖创意工作室，尤其擅长做三维材质碰撞和硬核产品广告，画面的光影质感好到让人头皮发麻。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：产品广告/3D质感；研究材质与光影
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「ManvsMachine」

**24. Oddfellows** — https://oddfellows.tv/
- 定位/资源类型：工作室官网；领域标签：动态、插画
- 主要内容：插画风与2D角色动画工作室（官网地址显示 Portland）
- 原文要点（摘录）：美国工作室，主打插画风和 2D 角色动画，配色极其舒服，镜头衔接和动作惯性做得丝滑无比。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：插画动画与品牌动态；学配色与动作惯性
- 核验：✅ 已核验（2026-11-15）curl 首次 TLS 断开、重试 202；WebFetch 取得作品列表正文

**25. Golden Wolf** — https://www.goldenwolf.tv/
- 定位/资源类型：工作室官网；领域标签：动画
- 主要内容：伦敦动画工作室
- 原文要点（摘录）：伦敦动画工作室，风格极好认——高饱和撞色、夸张的透视变形、快到飞起的剪辑节奏，满屏都是精力旺盛的街头卡通感。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：年轻化/潮流动画；学高能量配色与节奏
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Golden Wolf」

**26. Ordinary Folk** — https://www.ordinaryfolk.co/
- 定位/资源类型：工作室官网；领域标签：动态
- 主要内容：温哥华动态团队，2D几何图形动画
- 原文要点（摘录）：温哥华的团队，专门把基础的 2D 几何图形玩出花来，运动曲线的弹性和节奏感拿捏得死死的。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：几何动态/信息动效；学运动曲线
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Ordinary Folk – Motion Design & Animation Studio, 」

### 三、3D 与渲染（9 个）

**27. ArtStation** — https://www.artstation.com/
- 定位/资源类型：作品集/社区；领域标签：3D、游戏
- 主要内容：CG/游戏美术作品社区
- 原文要点（摘录）：干 CG 和游戏美术的人每天开机必逛的地方。全球各大游戏厂、影视视效公司的原画师、建模师、灯光师基本都在这儿安家，搜任何风格的概念设计或三维资产都能找到最顶级的参考。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：CG/游戏美术参考；搜风格化概念设计
- 核验：✅ 已核验（2026-11-15）curl 403（Cloudflare challenge）、WebFetch 500；无头 Chrome 渲染出首页

**28. The Rookies** — https://www.therookies.co/
- 定位/资源类型：社区/赛事；领域标签：3D、游戏
- 主要内容：面向学生与新人的年度比赛社区
- 原文要点（摘录）：专门给全球相关专业大学生和入行新人办的年度比赛社区，分 3D 动画、游戏开发、视觉特效、概念设计好几个赛道。刚学软件或者准备找工作的人可以去翻翻，看看现在的应届生作品集都已经卷到什么地步了。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：作品集对标；看应届作品水平
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「The Rookies - Creative Community for Next-Gen Arti」

**29. 80 Level** — https://80.lv/
- 定位/资源类型：媒体/3D；领域标签：3D、游戏
- 主要内容：游戏美术与三维技术媒体，Breakdown 制作拆解
- 原文要点（摘录）：专聊游戏美术和三维技术的媒体。这个站最值得看的是它的 Breakdown（制作拆解）文章：请原作者出面，把一个复杂的三维场景拆开，从用什么软件建白模、怎么在 Substance 里刷脏迹，到怎么在引擎里摆灯光，写得跟操作手册一样细。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：3D制作流程学习；读 Breakdown
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「80 Level」

**30. Sketchfab** — https://sketchfab.com/
- 定位/资源类型：平台/3D资产；领域标签：3D
- 主要内容：网页3D模型查看与发布平台（可切线框/法线）
- 原文要点（摘录）：直接在网页上 360 度转着看 3D 模型的平台。遇到做得好的模型，点一下右下角的查看器设置，就能直接切到纯白模、线框（Wireframe）、法线贴图或者粗糙度通道——别人模型是怎么布线的、UV 怎么拆的，扒得干干净净。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：看布线与贴图通道；拆模型结构
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Sketchfab - The best 3D viewer on the web」

**31. befores & afters** — https://beforesandafters.com/
- 定位/资源类型：媒体/VFX；领域标签：VFX、影视
- 主要内容：好莱坞视效幕后杂志
- 原文要点（摘录）：专门扒好莱坞大片视效幕后的在线杂志。文章最爱放特效前后的对比图：左边是演员穿着动作捕捉服站在绿幕前，右边是合成完的爆炸场面，同时配着视效总监的采访，讲清楚这场戏到底是怎么借位和合成的。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：VFX流程学习；看前后对比
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「befores & afters - VFX magazine」

**32. fxguide** — https://www.fxguide.com/
- 定位/资源类型：媒体/VFX；领域标签：VFX、影视
- 主要内容：资深影视视效技术媒体
- 原文要点（摘录）：圈内资历最老的影视视效技术媒体。文章写得非常硬核，不聊八卦，专门深挖渲染器底层算法、虚拟制片 LED 棚管线、流体解算技术，适合想往技术美术（TA）或视效深水区走的人。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：技术美术进阶；读技术深文
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「fxguide」

**33. Blender Studio** — https://studio.blender.org/
- 定位/资源类型：教程/资产；领域标签：3D
- 主要内容：Blender 官方开源动画工作室，教程与工程文件（付费）
- 原文要点（摘录）：Blender 官方自己的开源动画工作室（付费）。官方团队每年都会用 Blender 做一部高质量动画短片来测试软件极限，订阅之后不仅能看教程，还能把他们做片子用的角色绑定、灯光工程文件直接下到自己电脑里打开研究。
- 价格：付费/部分付费
- 使用场景与价值：Blender 学习；下载工程文件拆解
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Blender Studio」

**34. Poly Haven** — https://polyhaven.com/
- 定位/资源类型：素材/3D资产；领域标签：3D、素材
- 主要内容：CC0 免费 HDRI、PBR 材质、扫描模型
- 原文要点（摘录）：做三维渲染必存的良心资源站。里面的高清 HDRI 环境光贴图、PBR 材质球和扫描模型全部采用 CC0 协议——意思是完全免费、不用注册就能直接下载，拿去接商业私活也不用署名。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：3D渲染素材；下载 HDRI/材质
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Poly Haven」

**35. Beeple Everydays** — https://beeple-crap.com/everydays
- 定位/资源类型：作品集/数字艺术；领域标签：3D、数字艺术
- 主要内容：Beeple 自2007年起的每日一图（页面显示 7,137 天）
- 原文要点（摘录）：数字艺术家 Beeple 从 2007 年 5 月 1 日那天起，逼自己每天做一张图传上网，结婚、生病、过年一天都没断过，就这么连着画了快二十年。你如果往前翻他头两年的图，会发现画得也挺糙的，但一页页往后翻，能亲眼看到一个普通人是怎么靠每天交作业硬生生把自己练成大神的。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：数字艺术/坚持练习；看长期练习轨迹
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Everydays ／ BEEPLE」

### 四、电影画面与镜头参考（7 个）

**36. ShotDeck** — https://shotdeck.com/
- 定位/资源类型：截图库/影视；领域标签：影视、摄影
- 主要内容：电影截图库，官网称150万+可检索镜头（付费）
- 原文要点（摘录）：《小丑》《宿醉》的摄影指导 Lawrence Sher 带头做出来的专业电影截图库（付费）。图库极其庞大，而且每张图的标签打得细到离谱：你可以直接筛选「黄金时刻 + 逆光 + 广角镜头 + 冷色调 + 车内景」，一秒钟就能拉出几十张完全符合要求的电影画面拿去做分镜参考。
- 价格：付费/部分付费
- 使用场景与价值：电影感布光/构图参考；按光线/镜头/色调筛
- 核验：✅ 已核验（2026-11-15）curl 403（Cloudflare）；WebFetch 取得首页正文

**37. FILMGRAB** — https://film-grab.com/
- 定位/资源类型：截图库/影视；领域标签：影视
- 主要内容：免费电影截图站，一片一页
- 原文要点（摘录）：完全免费的电影截图网站，收了几千部经典电影。它的整理方式很纯粹：一部电影就是一个单独的页面，里面整整齐齐摆着从片中挑出来的五六十张高清关键帧。想研究某位导演的用光和构图习惯，点进一页从头划到底就全明白了。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：研究导演用光构图；整片关键帧对比
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「[FILMGRAB]」

**38. StillsLab** — https://stillslab.com/
- 定位/资源类型：截图库/影视；领域标签：影视
- 主要内容：免费影视截图库，细标签+统计（如夜景占比）
- 原文要点（摘录）：免费的影视截图库，电影、剧集、MV、广告都有，不付钱也能看全库。标签打得很细，可以按景别、机位角度、光线、色彩、日景夜景，甚至用的什么摄影机和镜头来筛，也能直接敲一句大白话描述画面去搜。每部片子的页面还会给出统计，比如《银翼杀手 2049》里夜景占 69%、柔光占 52%，研究一部片子的视觉配方特别方便。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：视觉配方研究；按景别/光线筛选
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「StillsLab — Movie Stills & TV Show Frames for Film」

**39. Flim** — https://flim.ai/
- 定位/资源类型：截图库/AI搜索；领域标签：影视、AI
- 主要内容：AI 语义搜索影视截图
- 原文要点（摘录）：接了 AI 语义搜索的影视截图库，除了电影还收了不少 MV 和商业广告。最好用的一点是不需要记片名，直接在搜索框里敲一句大白话（比如「一个人站在走廊尽头背光」或者「俯拍餐桌上的食物」），就能把各个片子里的类似镜头全搜出来。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：用自然语言找镜头；描述画面搜索
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Flim ／ AI search engine for film stills and visual」

**40. EyeCannndy** — https://eyecannndy.com/
- 定位/资源类型：词典/影视；领域标签：影视、视频
- 主要内容：镜头语言与剪辑技法动图词典
- 原文要点（摘录）：一个把「镜头语言和剪辑手法」做成动图词典的网站。看到好看的转场或运镜叫不出名字很正常，这里把匹配剪辑（Match Cut）、希区柯克变焦、鞭甩转场、第一人称视角等几十种常见技法全列了出来，点开一个词条，直接给你看五六个不同广告和MV里的动图实例。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：给技法命名、写AI视频提示词；查技法名称
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Eyecandy - Visual Technique Library」

**41. StudioBinder 镜头语言指南** — https://www.studiobinder.com/blog/ultimate-guide-to-camera-shots/
- 定位/资源类型：教程/影视；领域标签：影视、AI
- 主要内容：景别/机位/运镜系统教程
- 原文要点（摘录）：一家做制片软件的公司写的系列教程，把景别、机位角度、运镜方式（推拉、摇移、甩镜头、环绕）一种一种讲清楚，每一种都配了电影里的实例。审美高度一般，但胜在系统、好查。用 AI 生成视频时，提示词里写「low angle」「dolly in」「whip pan」比写「拍得高级一点」管用得多，这些词在这里都能查到。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：AI视频提示词术语；查 low angle、dolly in 等
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「50+ Types of Camera Shots, Angles, and Techniques」

**42. American Cinematographer（ASC）** — https://theasc.com/
- 定位/资源类型：媒体/摄影；领域标签：影视、摄影
- 主要内容：美国电影摄影师协会杂志与站点
- 原文要点（摘录）：美国电影摄影师协会（ASC）办了一百多年的杂志。上面的文章大多是摄影指导亲自讲一部片子：为什么选这套镜头、用的什么机器、主光从哪儿打、调色怎么定。截图库告诉你画面长什么样，这里告诉你为什么这么拍。不少文章在官网免费就能读全文。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：理解'为什么这么拍'；读摄影指导文章
- 核验：🟡 部分核验（2026-11-15）curl 与无头浏览器均返回 Cloudflare 520；WebFetch 取得新闻标题（站点间歇性故障）

### 五、UI 设计（16 个）

**43. Mobbin** — https://mobbin.com/
- 定位/资源类型：截图库/UI；领域标签：UI、移动端
- 主要内容：真实App截图库（原文称60万+界面，付费，免费号可看部分）
- 原文要点（摘录）：目前最好用的真实 App 截图库（付费，免费号能看一部分）。团队把海外大量主流 iOS、Android 和 Web 应用从头到尾截了个遍，攒了 60 多万张界面。当你要画一个「订阅付费页」或者「空状态提醒」时，直接上去筛这个功能标签，就能把 Airbnb、Spotify、Notion 的做法并排摆在一起对比。
- 价格：付费/部分付费
- 使用场景与价值：功能页对标（订阅页、空状态等）；按功能标签筛
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Mobbin — UI & UX design inspiration for mobile & w」

**44. Page Flows** — https://pageflows.com/
- 定位/资源类型：录屏库/UX；领域标签：UX
- 主要内容：真实产品操作录屏（付费）
- 原文要点（摘录）：Mobbin 看的是静态截图，而这个站存的全是真实产品的操作录屏（付费）。从新用户点开落地页、注册账号、绑卡付钱，一直到最后怎么找入口取消订阅，全程带着鼠标点击轨迹和页面跳转录下来，做交互流程梳理的时候极其省事。
- 价格：付费/部分付费
- 使用场景与价值：交互流程梳理；看注册/付费/取消流程
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「UI/UX Design Inspiration & User Flows from Top App」

**45. Refero** — https://refero.design/
- 定位/资源类型：截图库/UI；领域标签：UI、网页
- 主要内容：Web/iOS界面截图库，标签细（付费）；子站 styles.refero.design
- 原文要点（摘录）：专注 Web 网页端和 iOS 端的界面截图库（付费）。它的组件和页面类型标签切得非常碎，比如想单看别人怎么设计「表格筛选器」「面包屑导航」或者「价格对比表」，搜起来很准。它还有个免费子站 styles.refero.design，把两千多个真实网站的配色、字体、间距整理成了 AI 能直接读的 DESIGN.md，不登…
- 价格：付费/部分付费
- 使用场景与价值：组件/页面类型检索；搜具体组件
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Refero — UI/UX Design Inspiration for Your Next Pr」

**46. Nicelydone** — https://nicelydone.club/
- 定位/资源类型：截图库/UI；领域标签：UI、SaaS
- 主要内容：SaaS/Web应用界面库（付费）
- 原文要点（摘录）：专门收海外 Web 应用和 SaaS 软件界面的图库（付费）。平时做 ToB 业务、企业后台、工作台软件的人，看消费级 App 往往使不上劲，来这儿找复杂表单和数据看板的排版参考最合适。
- 价格：付费/部分付费
- 使用场景与价值：B端设计参考；找复杂表单/看板
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Nicelydone — Web apps design inspiration (UX & UI)」

**47. SaaSFrame** — https://www.saasframe.io/
- 定位/资源类型：截图库/UI；领域标签：UI、SaaS
- 主要内容：SaaS产品界面库（付费）
- 原文要点（摘录）：也是盯着 SaaS 产品收集的界面库（付费），把营销官网、登录注册页、功能弹窗、后台设置页分门别类理好了，很适合独立开发者和 B 端设计师翻阅。
- 价格：付费/部分付费
- 使用场景与价值：独立开发/B端；按页面类型翻
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「SaaSFrame - SaaS UI & UX Design Inspiration Librar」

**48. Figma Community** — https://www.figma.com/community
- 定位/资源类型：社区/源文件；领域标签：UI、工具
- 主要内容：Figma 开源社区：模板、插件、设计系统源文件
- 原文要点（摘录）：Figma 自带的开源社区。看别人的截图只能看个皮毛，在这里看到好的设计系统、大厂开源组件库或者排得漂亮的模板，点一下右上角的「Open in Figma」，整个源文件就直接进你草稿箱了。点开图层面板，别人怎么套的自动布局（Auto Layout）、怎么命名的颜色变量，一目了然。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：直接拆源文件；学 Auto Layout 与变量
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Discover community-made templates, plugins, and wi」

**49. Apple 人机界面指南（HIG）** — https://developer.apple.com/design/human-interface-guidelines/
- 定位/资源类型：规范文档；领域标签：UI、规范
- 主要内容：苹果官方设计规范
- 原文要点（摘录）：苹果官方写给设计师和开发者的规范文档。遇到「底部导航栏该放几个图标」「手指点击热区最小留多少像素」「什么情况下该弹警告框」这种基础问题，不用在网上到处问人，直接翻苹果这套文档，里面把原因讲得明明白白。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：iOS/macOS 设计依据；查规范
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Human Interface Guidelines ／ Apple Developer Docum」

**50. Material Design 3** — https://m3.material.io/
- 定位/资源类型：规范文档；领域标签：UI、规范
- 主要内容：Google 设计系统文档
- 原文要点（摘录）：Google 的设计系统文档。就算你平时不做原生安卓应用，这套文档也极力推荐通读一遍。它把一套大厂设计系统是怎么定色阶、怎么算字号层级、怎么处理深色模式对比度、怎么定义组件悬停和按下状态的逻辑，毫无保留地全写出来了。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：设计系统搭建；学色阶与状态逻辑
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Material Design」

**51. Vercel Web Interface Guidelines** — https://vercel.com/design/guidelines
- 定位/资源类型：规范清单；领域标签：网页、规范
- 主要内容：界面细节检查清单（交互/动画/布局/文案/表单/性能）
- 原文要点（摘录）：Vercel 整理的一份界面细节清单，交互、动画、布局、文案、表单、性能分门别类，每一条都是能直接照着检查的硬规矩，比如「手机上输入框字号不能小于 16px，不然 iOS 一点就会自动放大」「动画别偷懒写 transition: all」。最适合用 AI 写代码的人：页面上专门有一节教你接进 AI，给了现成的 AGEN…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：上线前自查；逐条检查
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Web Interface Guidelines」

**52. Impeccable** — https://impeccable.style/
- 定位/资源类型：AI设计工具；领域标签：AI、UI
- 主要内容：面向AI编码代理的'去AI味'设计 skill（原文称62项检查）
- 原文要点（摘录）：专门治「AI 味」的设计 skill。它把 AI 最爱用的默认套路列成了 62 项检查：米黄色的「AI 配色」、斜体衬线大标题、提示框左边一根彩色竖条、卡片里再套卡片、「01 Discover」这种编号小标题……装进 Claude Code、Cursor、Codex 之后，可以用它的命令让 AI 打磨排版、调布局、给自…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：约束AI生成UI；让Agent自查
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Impeccable: The missing design vocabulary for agen」

**53. The Component Gallery** — https://component.gallery/
- 定位/资源类型：组件库索引；领域标签：UI、设计系统
- 主要内容：跨设计系统组件对比（首页称60组件/95设计系统/2,671示例）
- 原文要点（摘录）：一个专门把各家大厂「基础组件」拉出来同台比武的网站。比如你想研究一个最普通的「开关（Toggle）」或者「警告横幅（Alert）」，点进去，它会把苹果、谷歌、微软、Shopify、GitHub 等几十套设计系统里的对应组件截图和文档链接全列在一页上，写组件规范时拿来查漏补缺特别爽。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：组件设计对标；同一组件多家对比
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「The Component Gallery」

**54. 60fps** — https://60fps.design/
- 定位/资源类型：动效库/UI；领域标签：UI、动效
- 主要内容：高帧率UI动效片段库
- 原文要点（摘录）：专门收集「丝滑 UI 动效」的网站。里面全是高帧率录下来的真实应用交互片段，没有花里胡哨的废话，打开网页满屏都是各种极有手感的卡片展开、下拉刷新和页面过渡动效。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：微交互灵感；找动效手感
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「60fps - UI/UX animation inspiration for mobile & w」

**55. Spotted in Prod** — https://www.spottedinprod.com/
- 定位/资源类型：动效库/UI；领域标签：UI、移动端
- 主要内容：已上线iOS应用的细节短视频
- 原文要点（摘录）：专门抓拍海外已上线 iOS 应用里那些「让人眼前一亮的小细节」。全是几秒钟的实机操作短视频，比如某个按钮按下去时的微弱震动反馈视觉化、或者一段藏在设置页里的小彩蛋，很适合平时抠细节找灵感。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：细节打磨；抠细节
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Spotted in Prod — The very best of iOS」

**56. Growth.Design** — https://growth.design/
- 定位/资源类型：案例/UX；领域标签：UX
- 主要内容：连环画形式拆解知名App体验
- 原文要点（摘录）：两个产品设计师做的网站，专门用「连环画」的形式拆解知名 App 的真实体验。比如他们会像普通用户一样去走一遍 Duolingo 的新手引导，或者去订一次 Airbnb，然后一页页画出来：这一步文案为什么能让人安心付钱，下一步弹窗又为什么会把人吓跑。既好玩又有干货。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：增长与转化设计；读案例学文案与心理
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Growth.Design — Better Products, Better Growth.」

**57. Laws of UX** — https://lawsofux.com/
- 定位/资源类型：知识卡片/UX；领域标签：UX
- 主要内容：UX心理学定律卡片
- 原文要点（摘录）：把交互设计里常被拿来装门面的心理学定律（比如菲茨定律、希克定律、米勒定律、峰终定律），浓缩成了二十几张干净的图文卡片。每点开一张，用三句话告诉你这定律是什么意思、最早是谁提出来的、落到具体界面设计上该注意什么。写改版方案需要找理论依据时，上去翻一下很快。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：写方案找依据；查定律
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Home ／ Laws of UX」

**58. Game UI Database** — https://www.gameuidatabase.com/
- 定位/资源类型：截图库/游戏UI；领域标签：UI、游戏
- 主要内容：游戏UI截图库（首页显示 1,997 款游戏/79,623 张截图）
- 原文要点（摘录）：一个规模吓人的游戏界面截图库，收了将近 2000 款主机与 PC 游戏、7 万多张高清截图。最牛的是它按 UI 功能做好了分类：你可以直接搜所有游戏里的「捏脸界面」「装备背包」「技能树」「任务弹窗」或「死亡结算画面」。哪怕不做游戏，去看看游戏设计师是怎么在极度复杂的信息量下排好视觉层级的，也相当涨见识。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：游戏UI参考；按功能搜界面
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Game UI Database 2.0 ／ Welcome」

### 六、网页灵感（10 个）

**59. Recent（原 Godly）** — https://recent.design/
- 定位/资源类型：网页灵感；领域标签：网页
- 主要内容：网页灵感库，缩略图即播滚动录屏（godly.website 301 跳转至此）
- 原文要点（摘录）：以前网页设计师几乎人手一个书签的 Godly（godly.website），现在输入原网址会直接跳转到这个新站 Recent。它保留了以前那种不用点进原网站、直接在缩略图上就能看高清滚动录屏的爽快体验，同时还把收录范围扩到了产品宣传片、App 图标、品牌视觉和海报。想看眼下海外独立开发者和科技公司最流行什么网页风向，刷…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：前沿网页灵感；看滚动录屏
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Recent — Design Inspiration」

**60. Siteinspire** — https://www.siteinspire.com/
- 定位/资源类型：网页灵感；领域标签：网页
- 主要内容：老牌网页灵感库，风格/类型/行业叠加筛选
- 原文要点（摘录）：办了十来年的老牌网页灵感库，攒了几千个站。它的筛选器做得很好用，可以把「视觉风格（如网格、极简、大字报）」「网站类型（如作品集、电商）」和「所属行业（如建筑、时尚）」叠在一起筛。整体选品眼光很克制，很少收那种眼花缭乱的炫技站，全是耐看的排版。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：克制型网页参考；按风格+行业筛
- 核验：✅ 已核验（2026-11-15）curl 429（Vercel Security Checkpoint）；WebFetch 取得作品列表

**61. Land-book** — https://land-book.com/
- 定位/资源类型：网页灵感/落地页；领域标签：网页
- 主要内容：落地页图库（含定价页/关于页/简历页）
- 原文要点（摘录）：专门收落地页（Landing Page）的图库。除了产品首页，里面也单独分出了定价页（Pricing）、关于我们、个人简历页的合集，做常规商业网站很实用。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：商业网站；按页面类型找
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Landbook - website design inspiration gallery」

**62. Landingfolio** — https://www.landingfolio.com/
- 定位/资源类型：网页灵感/区块；领域标签：网页
- 主要内容：落地页+区块拆解（原文称4600+区块，部分付费）
- 原文要点（摘录）：也是收落地页的图库，但多做了一步：把页面拆成了首屏、功能介绍、用户评价、行动按钮、页脚这些区块，一共 4600 多个，能复制成 Tailwind、Figma 或 Webflow 格式（部分付费）。拿来喂 AI 特别顺手——挑一个喜欢的区块丢给它，比用文字描述「给我做个好看的首屏」准得多。
- 价格：付费/部分付费
- 使用场景与价值：区块级参考、喂AI；复制区块结构
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「The Best Landing Page Design Inspiration, Template」

**63. awesome-design-md** — https://github.com/VoltAgent/awesome-design-md
- 定位/资源类型：AI设计规范；领域标签：AI、网页
- 主要内容：GitHub 开源合集：知名品牌网站的 DESIGN.md
- 原文要点（摘录）：GitHub 上的一个开源合集，把 Stripe、Linear、Vercel、Apple 这些公认好看的网站，各自的配色、字体、间距和组件风格整理成一份 DESIGN.md 文件。把它放进你的项目里，AI 就会照着这个品牌的规矩来生成界面，比你自己描述「我要 Linear 那种感觉」靠谱得多。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：让AI按品牌风格生成UI；放入项目约束AI
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「GitHub - VoltAgent/awesome-design-md: A collection」

**64. One Page Love** — https://onepagelove.com/
- 定位/资源类型：网页灵感；领域标签：网页
- 主要内容：单页网站合集与模板
- 原文要点（摘录）：专门收集「单页网站」的网站。有些小产品、线下活动或者个人主页，根本撑不起好几个频道的导航栏，去这儿看看别人是怎么在一页从上滑到下的篇幅里，把事情讲得清清楚楚又有节奏感的。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：单页/活动页；学单页节奏
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「One Page Love — One Page Website Inspiration and T」

**65. Minimal Gallery** — https://minimal.gallery/
- 定位/资源类型：网页灵感；领域标签：网页
- 主要内容：极简风格网站图库
- 原文要点（摘录）：只收极简主义风格网站的图库。如果总觉得自己排出来的页面塞得满满当当、透不过气，去这里多看几个站，学学别人是怎么单靠黑白灰、大留白和干净的字号对比把页面撑起来的。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：极简网页；学留白与层级
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Minimal Gallery – Hand-picked web design inspirati」

**66. Dark Mode Design** — https://www.darkmodedesign.com/
- 定位/资源类型：网页灵感；领域标签：网页
- 主要内容：只收深色模式网页
- 原文要点（摘录）：全网只收「深色模式」网页的图库。很多人做黑底网页容易要么漆黑一片分不清主次，要么发光特效加太多显得廉价。去这儿翻翻成熟案例，看看纯黑、深灰怎么拉开卡片层级，文字和细线边框该把透明度压到多少才不刺眼。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：深色界面；学深色层级
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Dark Mode Design 🌘 Handpicked website inspiration」

**67. Hoverstat.es** — https://www.hoverstat.es/
- 定位/资源类型：网页灵感；领域标签：网页
- 主要内容：另类/实验网页合集
- 原文要点（摘录）：专门收录「怪网站」的地方。里面基本看不到正经的商业公司官网，全是独立艺术家、先锋设计工作室、地下乐队或者实验建筑师的主页。导航栏藏在奇怪的地方、鼠标滑过去满屏乱飞——当你觉得现在的网页全都长一个样、看腻了套路的时候，去这儿逛逛会非常解闷。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：找反套路灵感；看实验网页
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「HOVERSTAT.ES ／ The home of alternative web-design.」

**68. Web Design Museum** — https://www.webdesignmuseum.org/
- 定位/资源类型：档案/网页史；领域标签：网页、历史
- 主要内容：1991–2006 网页设计历史档案
- 原文要点（摘录）：一个正儿八经的「网页设计历史博物馆」。站长把 1991 年到 2006 年之间几千个古早网站的截图全存了下来——你能看到 1997 年的苹果官网长什么样、千禧年前后的雅虎门户排得有多密，以及当年红极一时的拟物化按钮和 Flash 酷站。除了怀旧，现在很多潮牌爱玩的千禧年复古风（Y2K），来这儿直接就能翻到最纯正的一手史…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：复古网页/Y2K 参考；查年代视觉
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Web Design Museum – Discover old websites, apps, s」

### 七、前端与交互（16 个）

**69. Codrops** — https://tympanus.net/codrops/
- 定位/资源类型：教程/前端；领域标签：前端
- 主要内容：创意前端教程与 Demo
- 原文要点（摘录）：做创意前端的人必存的宝地。这个站常年分享各种能在 Awwwards 上拿奖的前端特效教程：WebGL 图片扭曲、丝滑的页面无刷新过渡、跟着滚动条变形的文字网格。最良心的是每一篇文章不仅把实现思路一步步讲清楚，还直接附上在线 Demo 和 GitHub 源码仓库。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：创意前端实现；照教程复现
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Codrops ／ Fueling web creativity since 2009」

**70. CodePen Spark** — https://codepen.io/spark
- 定位/资源类型：代码合集/前端；领域标签：前端
- 主要内容：CodePen 每周创意代码精选
- 原文要点（摘录）：CodePen 编辑部每周整理一次的创意代码合集。里面全是世界各地的前端用几百行 CSS、SVG 或 Canvas 写出来的小玩具。看中哪个效果，点进去左边就是 HTML/CSS/JS 源码框，随手改两个数字，右边画面当场就跟着变，拿来练手再好不过。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：找前端小特效；改参数学原理
- 核验：✅ 已核验（2026-11-15）curl 403（Cloudflare）；WebFetch 取得本周 Spark 列表

**71. GSAP 官方 Demo 库** — https://demos.gsap.com/
- 定位/资源类型：示例库/前端动画；领域标签：前端、动效
- 主要内容：GSAP 动画示例（滚动/文字/悬停等）
- 原文要点（摘录）：网页动画老大哥 GSAP（GreenSock）的官方示例库，一百多个效果按滚动、文字、悬停、鼠标跟随、轮播分好了类，每个都附 CodePen 源码。以前 GSAP 很多最好用的高级插件（比如做滚动绑定的 ScrollTrigger、拆字动画的 SplitText）是要掏钱买会员的，被 Webflow 收购之后，现在连带…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：网页动效实现；复制 CodePen 源码
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「GSAP Demo Hub」

**72. Three.js 官方示例** — https://threejs.org/examples/
- 定位/资源类型：示例库/WebGL；领域标签：前端、3D
- 主要内容：Three.js 数百个官方 Demo
- 原文要点（摘录）：想在浏览器里做 3D 效果，基本绕不开 Three.js。不用到处找野路子教程，先把官方这几百个在线 Demo 挨个点开看一遍——小到加载一个带骨骼动画的模型，大到海洋水面反射、物理碰撞、后期辉光通道，所有效果右下角都有个「源码」按钮，点开就是最标准的官方写法。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：Web3D 入门与查效果；查示例源码
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「three.js examples」

**73. Shadertoy** — https://www.shadertoy.com/
- 定位/资源类型：社区/图形学；领域标签：前端、图形
- 主要内容：GLSL 着色器作品社区
- 原文要点（摘录）：图形学大神炫技的地方。这个网站里的所有酷炫画面——不管是翻滚的体积云、逼真的水波折射，还是一整座霓虹闪烁的立体城市，全都不靠导入外部图片或 3D 模型，纯粹是用几百行数学公式（GLSL 着色器代码）在显卡里实时算出来的。网页右边直接放着源码，虽然满屏三角函数看着头大，但想做流体背景或研究图形学的人绝对绕不开。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：着色器灵感；看 shader 源码
- 核验：🟡 部分核验（2026-11-15）curl 403、无头浏览器遇安全校验；WebFetch 仅得标题'Shader of the Week'

**74. The Book of Shaders** — https://thebookofshaders.com/
- 定位/资源类型：教程/图形学；领域标签：前端、图形
- 主要内容：片元着色器互动教程（含中文版）
- 原文要点（摘录）：如果你点开上面的 Shadertoy 觉得像在看天书，那就先来读这本免费的在线互动教程（自带中文版）。作者把枯燥的片元着色器（Fragment Shaders）掰碎了，从怎么用一条数学公式画出一条线、一个圆、再到生成噪波纹理，每一段代码都可以直接在文章里边改数字边看图案变化，是公认最好的 Shader 启蒙书。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：学 shader 基础；跟教程练习
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「The Book of Shaders」

**75. Bruno Simon** — https://bruno-simon.com/
- 定位/资源类型：个人站/WebGL；领域标签：前端、3D
- 主要内容：可驾驶玩具车的3D作品集
- 原文要点（摘录）：法国开发者 Bruno Simon 的个人主页。别人的简历是一页 PDF，他的简历是让你在浏览器里直接开着一辆玩具车，在 3D 沙盘里横冲直撞，撞倒路牌就能看他的工作经历和项目。他写的《Three.js Journey》也是目前把 Web 3D 讲得最透彻的课程之一。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：创意作品集；体验游戏化交互
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Bruno's」

**76. Lusion** — https://lusion.co/
- 定位/资源类型：工作室官网；领域标签：前端、3D
- 主要内容：英国WebGL创意开发工作室
- 原文要点（摘录）：英国一家专门接高定创意开发的工作室。他们自己的官网本身就是目前 WebGL 网页交互的天花板之一——从页面加载、滚轮阻尼、三维粒子转场到音效配合，没有一帧是卡顿或多余的，值得每个前端打开慢慢观摩。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：高端互动网页；观摩交互细节
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Lusion - Award Winning 3D and Interactive Web Stud」

**77. Active Theory** — https://activetheory.net/
- 定位/资源类型：工作室官网；领域标签：前端、互动
- 主要内容：美国数字互动工作室
- 原文要点（摘录）：美国顶尖的数字互动工作室。像好几届 Google I/O 大会的线上互动体验、早几年 Spotify 年度听歌报告（Wrapped）的互动页，很多大厂刷屏级的技术营销项目背后都是他们在写代码。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：互动营销案例；看项目案例
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Active Theory · Creative Digital Experiences」

**78. Framer Gallery** — https://www.framer.com/gallery/
- 定位/资源类型：网页灵感/建站；领域标签：网页、无代码
- 主要内容：Framer 搭建的优秀网站合集
- 原文要点（摘录）：Framer 官方挑出来的优秀网站合集。Framer 的操作界面跟 Figma 几乎一模一样，但画完点一下发布就是个带真实代码的响应式网站。去这个画廊逛一圈，你就能知道现在一个不懂代码的设计师，单靠拖拽和自带组件能把网站动效做到什么程度。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：无代码建站参考；找可复刻模板
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Framer Gallery: Explore the best websites built wi」

**79. Motion 官方示例** — https://motion.dev/examples
- 定位/资源类型：示例库/前端动画；领域标签：前端、动效
- 主要内容：Motion（原 Framer Motion）动画示例（部分付费）
- 原文要点（摘录）：现在写 React 和 Vue 最常用的动画库 Motion（以前叫 Framer Motion）的官方示例页。从最基础的弹簧物理缓动、列表增删重排，到复杂的跟随滚动条动画，常用的 UI 动效基本都有现成的简短示例（部分付费）：所有示例都能看演示，基础分类的一百多个免费给源码，复制过来就能改着用；其余的要买 Motio…
- 价格：付费/部分付费
- 使用场景与价值：React/Vue 动效实现；复制示例
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Examples: React, JavaScript, and Vue animation sni」

**80. React Bits** — https://reactbits.dev/
- 定位/资源类型：组件库/前端；领域标签：前端
- 主要内容：免费开源 React 动画组件
- 原文要点（摘录）：一个完全免费开源的 React 动画组件小超市。里面全是现成封装好的视觉小零件：文字乱码浮现、鼠标磁性吸附按钮、流光卡片边框、动态流体背景。左边调好速度、颜色参数，右边直接复制代码贴进自己项目里，五分钟就能让干巴巴的页面活起来。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：快速加动效；复制组件
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「React Bits — Free Animated React Components」

**81. coss ui** — https://coss.com/ui
- 定位/资源类型：组件库/前端；领域标签：前端、UI
- 主要内容：Cal.com 设计系统（前身 Origin UI），Tailwind，MIT
- 原文要点（摘录）：开源日程工具 Cal.com 自家的设计系统，前身是不少人收藏过的 Origin UI。基于 Tailwind 写的，五十多个基础组件加五百多个现成的小模块，MIT 协议随便用。它的风格很克制，看着就像一个认真打磨过的真实产品，而不是又一个「深色背景 + 发光边框 + 光束特效」的 AI 创业公司官网。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：产品级组件；直接用组件
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「A modern React UI component library – coss ui」

**82. Josh W. Comeau** — https://www.joshwcomeau.com/
- 定位/资源类型：博客/教程；领域标签：前端
- 主要内容：交互式前端博客（CSS/动画/SVG）
- 原文要点（摘录）：前端开发者 Josh Comeau 的博客。他讲 CSS 布局、弹簧动画、SVG 路径，不是干巴巴地贴代码，而是在文章里塞满能拖、能调参数的交互小图解，拖一下滑块你就明白为什么这条曲线看着更舒服。文章免费，进阶课程收费。原理看懂了，再让 AI 写动效时你才知道该提什么要求。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：CSS/动画原理；拖滑块理解原理
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Josh W. Comeau」

**83. Rauno Freiberg** — https://rauno.me/
- 定位/资源类型：个人站/交互；领域标签：前端、交互
- 主要内容：Vercel 设计工程师个人站，《Invisible Details of Interaction Design》
- 原文要点（摘录）：目前在 Vercel 担任设计工程师的 Rauno 的个人网站。强烈建议把他站里那篇《Invisible Details of Interaction Design》（交互设计中看不见的细节）从头到尾读一遍。他用十几个可以亲手点按的交互小组件，把「为什么苹果系统的滑动停下来那么自然」「下拉菜单怎么根据鼠标移动斜率防误触…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：交互细节学习；读交互细节文章
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Rauno Freiberg」

**84. Emil Kowalski** — https://emilkowal.ski/
- 定位/资源类型：博客/动效；领域标签：前端、动效
- 主要内容：Sonner/Vaul 作者博客，界面动画
- 原文要点（摘录）：很多前端都在用的开源提示框组件 Sonner 和抽屉组件 Vaul 的作者，之前在 Linear 做设计工程师。他的博客文章篇幅都不长，但全在死磕一个问题：怎么让界面动画显得「克制又跟手」。比如弹窗到底该用多少毫秒、什么情况下绝对不要加动画，读完能改掉不少乱加动效的坏毛病。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：动画时长/缓动调校；读动画文章
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Emil Kowalski」

### 八、字体与配色（10 个）

**85. Typewolf** — https://www.typewolf.com/
- 定位/资源类型：字体指南；领域标签：字体
- 主要内容：字体指南与真实网站字体搭配
- 原文要点（摘录）：海外排版圈公认最靠谱的字体指南网站。站长是个对字体极度挑剔的设计师，以前每天推荐一个把字体用得极好看的真实网站，并标出它主标题和正文分别用了什么字（2025 年底之后就没再更新了，但攒下的案例和榜单照样能翻）。此外，网站里整理的「十佳无衬线体」「Google Fonts 最佳搭配方案」含金量极高，做英文或中西混排页面拿…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：选字体搭配；查字体组合
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「What’s Trending in Type  · Typewolf」

**86. Fonts In Use** — https://fontsinuse.com/
- 定位/资源类型：字体档案；领域标签：字体、平面
- 主要内容：真实世界字体使用档案
- 原文要点（摘录）：一个靠全球设计师共同维护的「字体实战档案馆」。它不卖字库，专门收集现实世界里的海报、书籍封面、唱片封套、路牌、网页截图，然后像法医一样把里面用到的每一款字体名字全扒出来标在旁边。你想知道某款字体印在纸上或排在网页上到底是什么气质，搜一下它里面的真实案例就清楚了。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：看字体实际效果；按字体检索案例
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Fonts In Use - Fonts In Use」

**87. Google Fonts** — https://fonts.google.com/
- 定位/资源类型：字体库；领域标签：字体
- 主要内容：免费开源字库（含思源黑/宋等）
- 原文要点（摘录）：大家最熟悉的老朋友，完全免费可商用的开源字库。除了海量的英文字体，像中文里最常用的思源黑体（Noto Sans SC）、思源宋体（Noto Serif SC）、霞鹜文楷（繁体版）都能在上面直接下载，写前端更是连字体包都不用下，引一行链接就能跑。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：免费可商用字体；选字下载
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Browse Fonts - Google Fonts」

**88. Fontshare** — https://www.fontshare.com/
- 定位/资源类型：字体库；领域标签：字体
- 主要内容：ITF 免费字库（个人与商用免费）
- 原文要点（摘录）：印度知名字体大厂 ITF 办的免费字库网站。上面的字体虽然数量没有 Google Fonts 那么夸张，但款款都是精品，而且承诺 100% 免费供个人和商业项目使用。像这两年在海外独立网页和科技圈出镜率极高的几何无衬线体 Satoshi、标题字 Clash Display、General Sans，全是从这儿免费流出来…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：免费精品字体；选几何无衬线
- 核验：✅ 已核验（2026-11-15）curl HTTP 200（gzip 正文）；无头截图正常

**89. Butterick's Practical Typography** — https://practicaltypography.com/
- 定位/资源类型：教程/排版；领域标签：字体、排版
- 主要内容：免费在线排版书
- 原文要点（摘录）：一本写得极其痛快的免费在线排版小书。作者既写过代码又当过职业字体设计师，书里没有任何故弄玄虚的艺术理论，上来就用「10 分钟掌握排版核心」一章直接给你划硬指标：正文一行控制在多少个字母最舒服、行高设多少倍、为什么绝对不要随便拉宽字间距。哪怕只读完这第一章，你排出来的文档和网页都会立马顺眼一大截。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：排版基础；读'10分钟'章节
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Butterick’s Practical Typography」

**90. Utopia** — https://utopia.fyi/
- 定位/资源类型：工具/排版；领域标签：字体、前端
- 主要内容：流体字号/间距比例计算器
- 原文要点（摘录）：很多新手画页面时，大标题设 32px、小标题设 22px、正文设 14px，全是拍脑袋瞎填的，最后页面看着毫无秩序。这个小工具就是帮你按「数学比例」定字号的：分别填好手机和电脑上的正文字号，再选一个缩放倍率（比如大三度 1.250），它自动算出一整套会随屏幕宽度平滑缩放的字号变量，间距也能一起算。免费、不用注册，生成的…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：建立字号系统；生成 CSS 变量
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Fluid Responsive Design ／ Utopia」

**91. Coolors** — https://coolors.co/
- 定位/资源类型：工具/配色；领域标签：配色
- 主要内容：配色生成器（空格随机、锁色、色盲模拟）
- 原文要点（摘录）：最好用的傻瓜式配色工具。打开网页什么都不用设置，直接敲键盘空格键，屏幕上就会随机刷出一组五色卡；看到顺眼的颜色点一下锁头把它锁死，再继续敲空格，算法就会自动围绕你锁住的颜色去配剩下的颜色。支持一键模拟色盲用户眼里的画面，还能直接把色卡导出成图片或代码。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：快速配色；生成并导出色卡
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Coolors - The super fast color palettes generator!」

**92. Realtime Colors** — https://www.realtimecolors.com/
- 定位/资源类型：工具/配色；领域标签：配色
- 主要内容：在真实页面上实时预览配色（原文描述）
- 原文要点（摘录）：存了一堆好看的五色卡，真到画页面时还是抓瞎——不知道哪个色填背景、哪个色涂按钮、哪个色写正文。这个工具解决的就是这个痛点：你可以在底部工具栏自己挑（或者随机摇出）文字色、背景色、主色、次色和强调色，上面的标准落地页和后台图表会实时跟着变色，还能随时点一下太阳/月亮图标看这套颜色切到深色模式会不会翻车。调好之后能直接导出…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：配色落地预览（当前不可用）；暂用 Coolors+Radix 替代
- 核验：❌ 访问失败（2026-11-15）HTTP 402 DEPLOYMENT_DISABLED，页面显示'This deployment is temporarily paused'（站点部署被暂停，非网络问题）

**93. Radix Colors** — https://www.radix-ui.com/colors
- 定位/资源类型：工具/配色；领域标签：配色、设计系统
- 主要内容：12级界面色阶系统
- 原文要点（摘录）：开源组件库 Radix 配套的一整套界面配色。它给的不是几组好看的色卡，而是把每种颜色拆成 12 级，并且规定好了每一级干什么用：哪几级当背景、哪几级给按钮悬停、哪几级画边框、哪几级写文字，深色模式也一并配好了。照着这套规矩用色，页面很难乱；跟 AI 说一句「颜色按 Radix 的 12 级来用」，也比说「配色高级一点…
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：设计系统配色；按级取色
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Radix Colors」

**94. tweakcn** — https://tweakcn.com/
- 定位/资源类型：工具/主题；领域标签：前端、配色
- 主要内容：shadcn/ui 可视化主题编辑器
- 原文要点（摘录）：现在用 AI 写前端，很多人用的都是 shadcn/ui 这套组件，结果就是满大街的网站长得一模一样——这也是作者做它的原因。tweakcn 是给 shadcn 换皮的可视化编辑器：颜色、字体、圆角、阴影在左边调，右边的卡片、表单、仪表盘实时变样，还有一堆预设主题可以直接套，调满意了导出主题代码贴进项目就行。免费开源。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：避免 shadcn 同质化；调主题导出
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Beautiful themes for shadcn/ui — tweakcn ／ Theme E」

### 九、日常收集灵感（6 个）

**95. Pinterest** — https://www.pinterest.com/
- 定位/资源类型：灵感收集；领域标签：综合
- 主要内容：全网最大图片灵感平台
- 原文要点（摘录）：图库体量依然是全网第一，尤其适合顺藤摸瓜：找准一张对味的参考图点进去，顺着底下的「相似图片」一路往下点，十分钟就能拉出几十张同风格的图。缺点是这两年首页信息流里混进了不少粗糙的 AI 生成图和营销号杂图，建议建几个私密画板（Board），只钉真正精挑细选过的好图，把推荐算法慢慢养干净。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：情绪板、顺藤摸瓜找同风格；相似图扩展
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Pinterest」

**96. Are.na** — https://www.are.na/
- 定位/资源类型：灵感收集；领域标签：综合
- 主要内容：无算法、无点赞的研究型收集工具
- 原文要点（摘录）：设计圈里很多极客、建筑师和独立撰稿人偏爱的资料收集工具。它长得非常素，没有广告、没有算法信息流、甚至连「点赞数」都没有。你可以建不同的频道（Channel），把图片、PDF 文献、网页链接、随手记的一段话塞进去，还能把自己的频道跟全世界其他人的公开频道串联起来。很适合安安静静攒某个特定课题的研究资料。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：课题研究攒资料；建频道串联
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Are.na」

**97. Cosmos** — https://www.cosmos.so/
- 定位/资源类型：灵感收集；领域标签：综合
- 主要内容：新一代灵感收藏夹（浏览器插件）
- 原文要点（摘录）：这两年在海外设计师圈子里蹿红的新一代灵感收藏夹。装上它的浏览器插件，平时在推特或任何网站上看到好图、好视频，右键一下就能收进自己的空间。它的界面排版极其干净，而且因为早期用户大多是审美在线的创意人，直接在它的发现页（Discover）里逛别人公开的收藏夹，图片质量非常高。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：收集好图视频；逛 Discover
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Cosmos」

**98. Savee** — https://savee.com/
- 定位/资源类型：灵感收集；领域标签：平面、品牌
- 主要内容：极简图片灵感社区
- 原文要点（摘录）：专门做给视觉设计师看的极简图片社区。打开网站连多余的文字标题都没有，满屏就是干干净净的高清大图瀑布流。上面沉淀的内容非常纯粹，基本集中在平面排版、品牌包装、先锋摄影、字体设计和工业造型，想找高级感平面参考时，来这儿刷比去综合平台效率高得多。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：高级感平面参考；刷瀑布流
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Savee」

**99. It's Nice That** — https://www.itsnicethat.com/
- 定位/资源类型：媒体/创意；领域标签：平面、插画
- 主要内容：伦敦创意文化媒体
- 原文要点（摘录）：伦敦办了很多年的创意文化媒体。每天更新几篇短文章，聊全球各地最新的插画、平面、动画、摄影项目。它好看的地方在于不光贴图，编辑很会挖创作者背后的好玩故事——比如这个奇怪的字体是怎么因为一次印刷失误弄出来的、那支荒诞的短片导演当时在想什么。很适合当午饭时的电子榨菜。
- 价格：可免费浏览（原文未标付费）
- 使用场景与价值：创意文化阅读；午间阅读
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「It's Nice That」

**100. Brand New** — https://www.underconsideration.com/brandnew/
- 定位/资源类型：媒体/品牌；领域标签：品牌
- 主要内容：品牌换标点评（付费，免费可见新旧 Logo 对比）
- 原文要点（摘录）：全球品牌换标（Rebranding）的专业点评网站。只要国内外稍微有点名气的公司、大学、体育联赛或者消费品换了新 Logo 和新视觉系统，这里就会第一时间把旧版和新版并排摆出来，从字体微调、图形演变到实际延展应用做一番客观（有时相当毒舌）的拆解，底下还有全球同行投票打分（付费，不订阅只能看到新旧 Logo 的对比图）。…
- 价格：付费/部分付费
- 使用场景与价值：品牌设计判断力；看新旧对比
- 核验：✅ 已核验（2026-11-15）curl HTTP 200，页面标题「Brand New」

## 文章之外补充（扩展 15 个，不计入 100）

> 以下为补充收录的中文站与常用站，统一归类为「文章之外补充」。

| # | 网站名称 | 链接 | 主要内容 | 资源类型 | 设计特点 | 推荐用途 | 信息核验情况 |
|---|---|---|---|---|---|---|---|
| S1 | Behance（主站）（文章之外补充） | https://www.behance.net/ | Adobe 旗下作品集平台 | 作品集 | 全领域多元风格 | 作品集/找设计师 | ✅ 已核验：curl/WebFetch 403；无头 Chrome 渲染出首页 |
| S2 | Dribbble（文章之外补充） | https://dribbble.com/ | 设计师作品 shot 社区 | 作品集 | 扁平插画、UI概念稿、3D、渐变 | UI/插画灵感 | ✅ 已核验：curl 202 空页、WebFetch 403；无头 Chrome 渲染出首页 |
| S3 | 站酷 ZCOOL（文章之外补充） | https://www.zcool.com.cn/ | 中文设计师作品社区 | 作品集 | 商业插画、海报、电商、国潮 | 中文商业设计参考 | ✅ 已核验：curl HTTP 200，页面标题「站酷ZCOOL-设计师互动平台，设计师们都在站酷」 |
| S4 | 花瓣网（文章之外补充） | https://huaban.com/ | 中文图片采集与画板 | 灵感收集 | 电商营销、海报、古风/国潮插画（首页画板可见） | 中文情绪板 | ✅ 已核验：curl 返回 JS 反爬脚本；WebFetch 取得首页正文 |
| S5 | UI中国（文章之外补充） | https://www.ui.cn/ | 中文 UI/交互作品社区 | 作品集 | 移动端UI、Banner、图标 | 中文UI参考 | ❌ 访问失败：curl TLS 断开/HTTP2 PROTOCOL_ERROR，WebFetch 500；域名在本机解析到 198.18.0.1（代理保留段），疑为测试环境网络问题，非站点确定下线 |
| S6 | 优设网（文章之外补充） | https://www.uisdc.com/ | 中文设计教程/AIGC 教程媒体 | 教程/媒体 | 设计教程、AIGC 提示词 | 中文教程与AI绘图教程 | ✅ 已核验：curl HTTP 200，页面标题「优设网官网 - UISDC - 国内专业设计师平台 - 看设计文章，学AIGC教程，找灵感素材，尽在」 |
| S7 | Unsplash（文章之外补充） | https://unsplash.com/ | 免费高质量摄影图库 | 素材/摄影 | 自然、城市、生活方式摄影 | 免费配图 | 🟡 部分核验：返回浏览器校验页（.within.website 反爬），WebFetch 超时，无头浏览器停在校验页 |
| S8 | Pexels（文章之外补充） | https://www.pexels.com/ | 免费图片与视频素材 | 素材/摄影 | 生活方式摄影与视频 | 免费配图与视频 | ✅ 已核验：curl 403；WebFetch 取得首页正文 |
| S9 | Lapa Ninja（文章之外补充） | https://www.lapa.ninja/ | 落地页灵感（标题称 7,300+） | 网页灵感 | SaaS落地页 | 落地页参考 | ✅ 已核验：curl HTTP 200，页面标题「Landing Page Design Examples: 7,300+ Best Landing 」 |
| S10 | Designspiration（文章之外补充） | https://www.designspiration.com/ | 设计灵感图片收集，可按颜色搜索 | 灵感收集 | 平面、摄影、字体 | 按颜色找灵感 | ✅ 已核验：curl HTTP 200，页面标题「Designspiration - Design Inspiration ／ Inspiration」 |
| S11 | Color Hunt（文章之外补充） | https://colorhunt.co/ | 社区配色色卡 | 工具/配色 | 四色色卡 | 快速配色 | ✅ 已核验：curl HTTP 200，页面标题「Color Hunt - Color Palettes for Designers and Arti」 |
| S12 | Brutalist Websites（文章之外补充） | https://brutalistwebsites.com/ | 野兽派网站合集 | 网页灵感 | 原始、粗粝、反精致 | 野兽派参考 | ✅ 已核验：curl HTTP 200，页面标题「Brutalist Websites」 |
| S13 | Httpster（文章之外补充） | https://httpster.net/ | 网页灵感合集 | 网页灵感 | 现代网页、大字 | 网页灵感 | ✅ 已核验：curl HTTP 200，页面标题「Website Design Inspiration ／ Httpster」 |
| S14 | Logo Design Love（文章之外补充） | https://www.logodesignlove.com/ | Logo 与品牌识别博客 | 媒体/品牌 | 经典标志设计 | Logo 设计参考 | ✅ 已核验：curl HTTP 200，页面标题「Logo Design Love ／ on logos, symbols, icons, and m」 |
| S15 | styles.refero.design（文章之外补充） | https://styles.refero.design/ | Refero 免费子站：真实网站的 DESIGN.md 风格库（原文提及） | AI设计规范 | 真实网站配色/字体/间距 | 喂给AI的风格规范 | ✅ 已核验：curl HTTP 200，页面标题「Website Styles & DESIGN.md Library ／ Refero Styles」 |
