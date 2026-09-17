---
layout: default
title: "Horizon Summary: 2026-09-17 (ZH)"
date: 2026-09-17
lang: zh
---

> 从 38 条内容中筛选出 2 条重要资讯。

---

**科技博客**
1. [怀念旧版 Edge：从 EdgeHTML 之死看内核单一化](#item-tech-blog-1) ⭐️ 6.0/10
2. [iPadOS 27 新特性一览：Liquid Glass 微调与性能提升](#item-tech-blog-2) ⭐️ 4.0/10

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [怀念旧版 Edge：从 EdgeHTML 之死看内核单一化](https://sspai.com/post/113295) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · 9月16日 02:38

**「背景」** 2026 年 3 月 9 日是旧版 Edge（Edge Legacy）停止支持五周年。作者指出，尽管它常被调侃为「下载 Chrome 的工具」，但其基于 EdgeHTML 与 Chakra 的独立内核曾带来至今难以复现的体验，而它的退场也折射出浏览器内核多样性的式微。

**「方案」** 作者回顾了 EdgeHTML 的兴衰：微软为摆脱 IE 的兼容性包袱，于 2015 年随 Windows 10 推出全新内核，优先实现现实网站共用的 API，并深度绑定 Windows 系统 API（Media Foundation、DirectWrite、WinRT PDF 等），从而获得出色的性能与功耗表现。其滚动体验尤为突出——借助 DirectComposition 与 Direct Manipulation 实现异步滚动，为输入添加速度曲线，并根据容器尺寸计算滚动量，作者称这是当时最平滑的滚动；EPUB 阅读器也因可重排分页、墨迹批注和完整浏览器能力而被作者视为最佳。然而，与操作系统强绑定意味着无法移植，发版节奏受制于 Windows 半年更新，企业延迟部署导致版本长期落后，扩展生态不成熟又形成「用户少—开发者不测试」的恶性循环，UWP 平台的不成熟进一步拖慢迭代。最终微软为兼容性、跨平台和独立发版而转向 Chromium，作者认为这在商业上无比正确。文章随后将这一历史与当下联系起来：Chrome 停用 Manifest V2 后，Edge Chromium 等下游浏览器因 backport 成本高昂而陆续跟进，XSLT 也被移除，作者担忧近 90% 的浏览器被同一上游左右，而 Firefox 与 Safari 的份额不足以制衡。

**「启示」** 作者的核心论点是：独立浏览器内核本身就是价值，EdgeHTML 的消亡不仅是产品更替，更让互联网失去了一个制衡 Chromium 单一化的选项；当上游可以单方面决定 Manifest V2、XSLT 等功能的存废时，下游和用户都无能为力。

**标签**: `#browser-engines`, `#edgehtml`, `#chromium-monoculture`, `#web-standards`, `#manifest-v2`

---

<a id="item-tech-blog-2"></a>
### [iPadOS 27 新特性一览：Liquid Glass 微调与性能提升](https://sspai.com/post/114607) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · 9月16日 07:00

**「背景」** Apple 于 9 月 15 日凌晨发布 iPadOS 27 正式版，与 iOS 27、macOS 27 Golden Gate、watchOS 27 同步推出。少数派编辑部以更新日志式的视角，梳理了新版系统中界面、性能、Apple Pencil 与 AI 等方面值得关注的改动，供已升级或仍在观望的用户参考。

**「方案」** 界面方面，Liquid Glass 设计继续微调：应用侧边栏从 iPadOS 26 的悬浮样式回归 iPadOS 18 的边到边布局，与 macOS 27 保持一致；系统自带 app 图标基本全部重构，第三方图标渲染也更立体锐利；按钮、通知、输入框等组件换用新的光影渲染，被遮盖内容的折射减弱，可读性有所提升；设置中还新增了透明度调节滑块，最不透明档接近 iPadOS 18 的乳白毛玻璃效果。作者认为这些改动多属细节微调，部分甚至像「开倒车」，但也承认设计评价本就见仁见智。菜单栏改为默认只显示 app 名称、轻点才展开，以减少误触，同时基本移除了此前效果不佳的 SF Symbols 小图标，仅保留窗口操作图标。主屏幕编辑支持撤销重做，iPhone app 窗口可更自由地调整尺寸，Sidecar 随航新增 iPad 触屏多指手势操作。Apple Pencil 获得新的充电提示音，手写内容可被 Spotlight 索引并全文搜索，且依赖 PencilKit，第三方 app 同样受益；备忘录内容可拷贝为 Markdown。性能上，作者称动画与系统流畅度提升，部分机型待机续航改善，AirDrop、AirPlay 与外置 SSD 传输更快，并给出实测：从硬盘复制 3.74G 文件到 iPad mini 内置存储约 5 秒，反向拷贝 21G 不到 30 秒，接近跑满 10Gbps 带宽。AI 方面，Apple Foundation Models 加入 Google Gemini 助力，Apple 仍称其为自研，并叠加 Agentic 能力与既有 API 形成 Siri AI，具备系统级上下文与屏幕感知；但国行 iPad 暂不支持 Apple Intelligence 及 Siri AI 相关功能。

**「启示」** 作者的整体感受是，iPadOS 27 在继续打磨 Liquid Glass 之外，也在性能、交互与功能上有所精进，Apple 似乎有意让 macOS 与 iPadOS 更加靠近。不过文中多数结论为描述性或作者主观判断，除文件传输计时外缺少基准测试与方法说明，实际收益仍待更多验证。

**标签**: `#iPadOS`, `#Apple`, `#UI design`, `#release notes`, `#consumer tech`

---