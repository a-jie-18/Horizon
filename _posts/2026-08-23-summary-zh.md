---
layout: default
title: "Horizon Summary: 2026-08-23 (ZH)"
date: 2026-08-23
lang: zh
---

> 从 34 条内容中筛选出 4 条重要资讯。

---

**科技博客**
1. [Surface Pro 7 改造：AI 辅助的 Linux 看板与工作站](#item-tech-blog-1) ⭐️ 7.0/10
2. [WinAirCast：让 Windows 与 HomePod 无缝互联](#item-tech-blog-2) ⭐️ 4.0/10
3. [好奇提问与倾听：对话中的关键技能](#item-tech-blog-3) ⭐️ 4.0/10
4. [告别智能手机：实用建议与替代方案](#item-tech-blog-4) ⭐️ 4.0/10

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [Surface Pro 7 改造：AI 辅助的 Linux 看板与工作站](https://sspai.com/prime/story/surface-pro-7-linux-ai-dashboard) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · 8月23日 07:25

**「背景」** 作者有一台闲置的 Surface Pro 7，在 Windows 11 下长时间亮屏会过热、跳屏，几乎不可用。受墨水屏看板启发，作者决定将其改造为桌边常亮的 AI 用量看板和轻量工作站，并全程借助 AI 辅助完成。

**「方案」** 作者首先与 AI 讨论确定了技术路线：使用 Ubuntu 24.04 LTS、Rufus 写盘、整盘格式化并启用 LUKS 全盘加密。重启前，让 AI 生成跨设备交接 Prompt，手机 AI 接管安装向导，通过拍照确认 UEFI 选项和写盘进度。进入系统后，终端 Agent 检查并安装了 linux-surface 内核（6.19.8-surface-3）及触控组件，但首次重启后触屏无效，原因是 MOK 签名未确认和 GRUB 引导顺序错误。Agent 重新导入密钥、调整引导顺序后成功。针对不插键盘无法输入 LUKS 密码的问题，Agent 指导使用 Clevis 基于 TPM2（PCR 7）实现自动解锁。最终，设备成为桌边看板，运行作者自研的 AI Usage Dashboard，并支持摸鱼和 SSH 轻量任务。

**「启示」** 作者认为，通过 AI 辅助的系统改造，闲置硬件得以充分利用，展示了 AI 在系统管理中的实用价值。

**标签**: `#Linux on Surface`, `#AI-assisted sysadmin`, `#TPM2 disk encryption`, `#linux-surface kernel`, `#hardware repurposing`

---

<a id="item-tech-blog-2"></a>
### [WinAirCast：让 Windows 与 HomePod 无缝互联](https://sspai.com/post/113002) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · 8月23日 03:00

**「背景」** Windows 原生不支持 AirPlay，导致 PC 用户难以将音频串流到 HomePod。现有第三方工具如 TuneBlade 和 AirParrot 存在高延迟、系统兼容性差、对 AirPlay 2 设备支持滞后等问题。

**「方案」** 作者介绍了 WinAirCast，一款用 Rust 从零重写协议栈的音频串流工具，原生支持 AirPlay 2 并兼容 AirPlay 1。它通过 PTP 微秒级时钟同步实现多设备分组同步，在实时流媒体模式下延迟可低至 45ms。软件提供集中管理界面、桌面悬浮窗和设备停靠栏，支持按设备配置推流参数，包括 ALAC 和 PCM 编码。此外，WinAirCast 内置十段图形均衡器，支持单应用捕获和虚拟声卡穿透 DRM，并利用 MMCSS Pro Audio 调度防止爆音。作者通过对比表展示了其在延迟、协议支持、功能丰富度上的优势，并强调其定价为 $2.99，提供十五天免费试用。

**「启示」** 作者认为 WinAirCast 打破了生态壁垒，为 Windows 用户提供了稳定、低延迟且现代化的音频串流方案，让 HomePod 等设备在 PC 环境中发挥价值。

**标签**: `#AirPlay`, `#Windows`, `#audio streaming`, `#HomePod`, `#product announcement`

---

<a id="item-tech-blog-3"></a>
### [好奇提问与倾听：对话中的关键技能](https://www.reddit.com/r/selfimprovement/comments/1vw8dls/this_is_the_1_skill_you_can_learn_for_conversions/) ⭐️ 4.0/10

reddit · r/selfimprovement · /u/yaboythewiseman · 8月23日 14:17

**「背景」** 作者是一名护士，每天要面对多位新病人，这迫使她掌握了与陌生人交谈的技巧。她发现许多人在对话中过于关注自己该说什么，而忽略了对方真正在意的是你是否关心他们。

**「方案」** 作者提出的核心方法是：找到你真正好奇的点，向对方提问，然后闭嘴倾听。她以自己为例，喜欢爱情故事，所以常问病人“家人在附近吗”，一旦对方透露已婚或有孩子，就追问相识、求婚、婚礼等细节。由于她真心感兴趣，对方会乐于分享，对话自然流畅。她强调，即使不善言辞，只要表现出兴趣并让对方主导话题，就能留下好印象。她还提到，掌握这一基础后，可以叠加更高级的技巧，如寻找共同点、让对方自我赞美等。

**「启示」** 作者认为，对话的关键不在于你说什么，而在于你是否真正关心对方的故事。通过好奇提问和专注倾听，任何人都能建立良好的沟通，这一技能是提升对话能力的基础。

**标签**: `#conversation`, `#communication`, `#nursing`, `#anecdotal`, `#self-improvement`

---

<a id="item-tech-blog-4"></a>
### [告别智能手机：实用建议与替代方案](https://www.reddit.com/r/selfimprovement/comments/1vwit6n/going_smartphone_free_tips/) ⭐️ 4.0/10

reddit · r/selfimprovement · /u/the\_noobcat · 8月23日 20:58

**「背景」** 作者长期尝试完全离线生活，但发现因工作、社交和日常需求难以实现，因此转向更现实的目标：减少屏幕时间、改用功能手机，并保留必要的智能功能。作者已成功停用社交媒体三个月，但仍有依赖智能手机的多种场景，如 NFC 支付、导航、健康追踪和通讯应用。

**「方案」** 作者列出了保留智能手机的主要原因，并逐一提出替代方案：NFC 支付可通过银行卡或电脑完成大额交易，日常小额支付可改用现金或实体卡；GPS 导航可改用离线地图或车载导航；健康追踪可改用专用手环或手表；经期日历可改用纸质记录或专用设备；Viber 和 WhatsApp 群组可通过电脑应用使用，但需保持手机号激活；音乐可回归离线播放；拍照可用带摄像头的功能手机；打车可通过电话或路边招手。作者还建议逐步实施这些替代方案，并寻求成功过渡者的经验分享。

**「启示」** 作者认为，完全脱离智能手机不现实，但通过有意识地替换核心功能，可以实现有限屏幕时间和更健康的生活方式。关键在于找到满足必要需求的替代工具，而非彻底放弃便利。

**标签**: `#digital minimalism`, `#dumb phone`, `#smartphone alternatives`, `#screen time`, `#personal productivity`

---