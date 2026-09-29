---
layout: default
title: "Horizon Summary: 2026-09-29 (ZH)"
date: 2026-09-29
lang: zh
---

> 从 45 条内容中筛选出 2 条重要资讯。

---

**科技博客**
1. [iPhone Duo 折叠屏交互设计的元原则](#item-tech-blog-1) ⭐️ 7.0/10
2. [Termux 上把 Android 手机变成随身开发服务器](#item-tech-blog-2) ⭐️ 6.0/10

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [iPhone Duo 折叠屏交互设计的元原则](https://sspai.com/post/114972) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · 9月28日 07:00

**「背景」** 折叠屏设备长期面临形态与场景的复杂性：从 Surface Duo 的早期尝试，到多数厂商仅把「适配」做成留白与排版的权宜之计，交互设计始终缺乏规范。作者由此关注 iPhone Duo 的交互方案，并试图从 Apple 官方规范与 WWDC 分享中追溯其设计逻辑。

**「方案」** 作者认为，Apple 的设计脉络可回溯到 1987 年 HIG 的第一章：人不是想用电脑，而是想搞定手头的事。沿着 Chan Karunamuni 在 2018 年《Designing Fluid Interfaces》、2023 年灵动岛、2025 年 Liquid Glass 三场分享，作者归纳出六条「元设计原则」——情境先行、过程可控、空间连贯、任务连续、反馈明确、经验迁移，并强调这是其个人归纳而非 Apple 官方理论。

这些原则在 Duo 上落到具体决策：以「书」为隐喻，半折使用、书脊连接两侧；展开动画中，正在展开的一侧先呈现柔化光色，随铰链角度逐渐清晰，与 Liquid Glass 的光线弯曲逻辑呼应（作者指出官方未公布具体渲染算法，模糊与角度的精确对应属推测）。Dock 与工具栏从上下移到右侧，理由是握持时拇指可达、外屏纵向空间有限，且控件始终与摄像头/灵动岛对齐，在开合与分屏镜像中保持锚点；同时 HIG 要求控件靠近其所影响的内容，因此分栏工具不会为整齐而全部搬到最右。铰链提供档位与连续角度两类数据，虚拟吉他案例展示角度可直接驱动音高，弹出框则随平摊、半折、笔记本式支起等情境在居中、右侧、上屏之间移动。

**「启示」** 作者的核心论点是：比起折痕这类硬件指标，Apple 在 Duo 上更值得关注的是把交互重新拉回「人正在做什么」的持续提问能力；「书」的隐喻与六条元原则，正是这种能力在折叠屏上的具体兑现。

**标签**: `#interaction-design`, `#folding-devices`, `#Apple-HIG`, `#WWDC`, `#UI-adaptation`

---

<a id="item-tech-blog-2"></a>
### [Termux 上把 Android 手机变成随身开发服务器](https://sspai.com/prime/story/dev-env-on-android-with-termux) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · 9月28日 09:33

**「背景」** 作者在折腾 Hermes、Pi 这类终端 AI Agent 时发现，手机是让 Agent 随时可用的最顺手设备：电脑不总在身边，租云服务器又要额外花钱，而 Android 手机随时有网有电，性能足以跑现代 Linux 命令行环境。但在 Android 上搭建这类环境有两个主要麻烦：系统杀后台，以及部分命令行工具在 Android 上的底层兼容问题。

**「方案」** 作者以小米 15 Ultra 为例，在不 root、不刷机的前提下记录整套配置。核心思路是先在 Termux 里跑起终端 Agent，再补上后台保活和内网穿透，让手机变成可 SSH 连入的随身小服务器。相比网页聊天框，终端 Agent 拥有本地 Shell 权限和文件环境，能直接跑脚本、解包大文件、只把核心片段发给模型，还能通过 termux-api 调用通知和剪贴板。安装上作者强调不要从应用商店下载 Termux，而应去 GitHub Releases 获取，以免签名冲突导致插件装不上，并建议先授权存储、换国内镜像源。随后安装 Python、clang、cmake、rust、git 等依赖，用 pip install -e .\[termux\] 拉取 Hermes Agent，首次启动进入交互式引导选择模型提供商（作者选了按量计费的 DeepSeek），再让 Agent 自己装好 nodejs、rust、uv、tmux、neovim、openssh 等工具链。作者还附了一张 2026 年主流 CLI AI 工具在 Termux 上的兼容表：Hermes 与 Pi 原生支持，OpenCode、Codex CLI 需社区补丁版，Grok Build 可源码编译，Cursor CLI 需 proot-distro 容器，Claude Code 暂无稳定方案。保活方面，作者给出三层配置：省电策略设为无限制、关闭锁屏清理、开启开发者选项中的停用子进程限制；若仍掉线，可循环播放 1 分钟静音 WAV 换取音频焦点，但需在脚本里判断蓝牙状态，避免抢占 A2DP 通道导致耳机无声。

**「启示」** 作者认为，Android 手机配合 Termux 足以承载终端 AI Agent 和轻量开发环境，真正的门槛不在性能，而在系统的进程查杀机制与工具链兼容性；只要针对性地做好保活与兼容处理，手机就能成为随时可连的随身服务器。

**标签**: `#Termux`, `#Android`, `#CLI AI agents`, `#mobile dev environment`, `#process keepalive`

---