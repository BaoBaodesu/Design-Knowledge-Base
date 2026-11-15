# 第一轮笔记：网站内容与定位（2026-11-15）
- 通过 X API（get_posts_by_id，含 article 字段）读取原帖：为 X 长文（Article），标题《100 个提升审美的设计网站大赏》，作者 Eian（@EianLu）。正文含 206 个链接实体（含重复），编号条目恰为 1–100，原文自述分 9 类：大赛与奖项 12、动态设计与视频 14、3D 与渲染 9、电影画面与镜头参考 7、UI 设计 16、网页灵感 10、前端与交互 16、字体与配色 10、日常收集灵感 6。解析结果与原文计数一致。
- 原文正文内另提及但不单独编号的名称：godly.website（已并入 #59 Recent）、styles.refero.design（#45 Refero 子站，列入扩展 S15）、Cal.com（#81 coss ui 母公司）、YouTube、Linear、Satoshi 字体等；未计为独立网站。
- 原文 100 个无重复 URL → 补充数量 0。按最初简报另加 15 个扩展站（站酷、花瓣、UI中国、优设、Behance 主站、Dribbble、Unsplash、Pexels 等），均标注「文章之外补充」。
- 核验流程：① curl（桌面 Chrome UA，25s 超时，跟随跳转）；② 非 2xx 用 WebFetch；③ 全部站点用无头 Chrome 截图（1280×860）。
- 失败/异常明细：见 data/verification.tsv。值得注意：godly.website → 301 到 http://recent.design/?ref=godly，该 http 地址 curl 返回 500，而 https://recent.design/ 正常（旧书签可能打不开，建议直接用新地址）。
- 付费标注沿用原文「（付费）」标记，未逐一打开定价页核验。
