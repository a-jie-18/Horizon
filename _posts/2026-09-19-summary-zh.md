---
layout: default
title: "Horizon Summary: 2026-09-19 (ZH)"
date: 2026-09-19
lang: zh
---

> 从 38 条内容中筛选出 2 条重要资讯。

---

**科技博客**
1. [让 AI Agent 持续获取个人健康数据的七种路径](#item-tech-blog-1) ⭐️ 7.0/10
2. [watchOS 27 上手：动态应用网格与智能叠放新变化](#item-tech-blog-2) ⭐️ 4.0/10

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [让 AI Agent 持续获取个人健康数据的七种路径](https://sspai.com/prime/story/how-to-obtain-data-for-agent-analysis) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · 9月18日 03:19

**「背景」** 作者在健身平台期萌生让 AI Agent「接管」身体的想法，但前提是 Agent 能持续拿到自己已在记录的健康数据。他把问题拆成数据获取、数据处理与结果可信度三部分，本文只处理第一步，并坦言仅实测了 Apple Health 与 Oura，其余厂商信息来自公开资料整理。

**「方案」** 作者先把健康数据分为三层：步数、心率、睡眠等基础记录，readiness、strain 等算法指标，以及饮食、训练感受等手工记录；来源则分为聚合平台（Apple Health、Health Connect、Google Health）、厂商或专业 App（Oura、Whoop、Garmin、训记、Hevy 等）和报告或手工记录。厂商通常只把部分数据同步给平台，复合指标往往保留在订阅产品内，因此选择路径前应先问：数据是否已进入聚合平台、平台字段是否够用。

据此他梳理出七种获取方式：一是在 ChatGPT、Claude 或国内蚂蚁阿福等 AI 产品内直接授权读取 Apple Health，省心但适合轻量分析；二是用 Strava MCP、训记 API Skill、Hevy API Key、Freddy 等连接器或中转服务，需确认字段、存储位置与退订后能否导出；三是从聚合平台持续导出，Apple Health 可用快捷指令、Health Push、Health Auto Export 或自写 App，Android 侧则厘清 Google Health、Health Connect 与正在退场的 Google Fit，并可用 Health Sync、Health Data Export；四是直接调用官方 API 或 SDK，如 Google Health API 与 CLI、Oura 和 Whoop 的开发者接口、Samsung Health Data SDK；五是国内厂商路径，华为 Health Service Kit 允许个人申请，小米、OPPO、vivo 的个人接口普遍有限。

文中给出多段配置提示词，强调让 Agent 先读官方文档、不要凭记忆写接口，并处理 OAuth 令牌刷新与持久化、增量拉取的判重键与断点续传、迟到数据与重复记录。作者提醒 Oura 已于 2025 年 12 月弃用 PAT、WHOOP 迁移新版 API，旧脚本多已失效；WHOOP 以 physiological cycle 而非自然日为单位，需先向 Agent 说明，否则会得到时间错位的分析。

**「启示」** 作者的核心结论是：让 Agent 分析身体数据，难点不在分析本身，而在于先判断数据在哪一层、哪一类来源，再据此选择聚合平台导出、连接器或官方 API，并提前处理授权、增量同步与单位定义等工程细节。本文只是系列第一篇，数据处理与结果可信度仍待后续讨论。

**标签**: `#health-data`, `#ai-agents`, `#apple-health`, `#api-integration`, `#personal-data`

---

<a id="item-tech-blog-2"></a>
### [watchOS 27 上手：动态应用网格与智能叠放新变化](https://sspai.com/post/114670) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · 9月18日 03:30

**「背景」** Apple 于 9 月 15 日凌晨发布 watchOS 27 正式版，支持 Apple Watch Series 9 及之后机型，并需搭配升级到 iOS 27 的 iPhone 11 或后续机型。少数派编辑部在升级后梳理了值得关注的新功能，供已升级或仍在观望的用户参考。

**「方案」** 作者上手后认为，watchOS 27 的改动集中在设计打磨与交互补全上。Liquid Glass 继续演化，按钮玻璃质感更有深度、浅色背景下对比度更高，高光轮廓改为与 iOS 一致的上下缘；玻璃控件模糊程度明显提高，但 iOS 上的强度调节滑杆并未下放，效果基本等同于 iOS 默认一档。按下数码表冠会先进入全新的动态应用网格，它把常用应用和推荐内容放在更显眼处，图标更大更易点选，也可向下旋转表冠切回传统网格；由于国内暂无法使用 Siri AI，新版 Siri 图标尚不可见。智能叠放变得更主动，会按时间、地点和使用场景把更可能需要的小组件前置，作者体验中常见于日历待办、降雨预报、常用 iMessage 联系人和运动后数据回顾。新增的单指捏合手势可打开当前选中的智能叠放小组件，双指捏合进入时外侧会出现银色高光提示选中，再捏合一次即可进入；作者指出该手势仅适用于智能叠放中已出现的小组件，不如双指捏合通用。查找 app 将查找设备、联系人和物品三个独立 app 整合为以地图为背景的单一 app，支持精准查找 iPhone、第二代 AirTag 和 AirPods Pro 3 等设备。AI 部分作者明确标注国内尚不可用，仅作前瞻梳理：Siri AI 首次登陆手腕，支持更短对话与开放式提问，并有独立 App 可跨 iPhone 与手表接续对话、调取个人数据；Workout Buddy 无需 iPhone 即可使用，新增配速、距离和训练时长进度对比，并会调取健身历史做纵向比较。其他更新包括经期追踪新增围绝经期和更年期支持、儿童账户设置流程更新、Apple Music 启动更快、体能训练步数与健康 App 同步、改进室内跑步和步行距离追踪精度、可能根据使用情况给出电池优化建议、水分检测算法升级、Wi-Fi 连接改善、App 扩展启动更快、Watch App 设置页重新设计、睡眠模式支持时区变更、新增 Siri 模块表盘以及 Wallet 访客钥匙支持。作者从体验出发称页面加载性能大幅改进、触控响应提升、续航有体感改善，但这些性能与续航结论均来自主观感受，未提供测量数据。

**「启示」** 作者认为 watchOS 27 更新虽不起眼，但带来了几项实用新功能并优化了性能，整体不错；最大争议在于仅兼容 Series 9、Series 10、Series 11、Ultra 2、Ultra 3 和 SE 3，早期 Apple Watch 无法享受这些优化。

**标签**: `#watchOS`, `#Apple Watch`, `#wearables`, `#feature roundup`, `#user experience`

---