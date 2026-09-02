---
layout: default
title: "Horizon Summary: 2026-09-02 (ZH)"
date: 2026-09-02
lang: zh
---

> 从 30 条内容中筛选出 3 条重要资讯。

---

**科技博客**
1. [用 PowerShell 自定义 Windows 更新暂停时间](#item-tech-blog-1) ⭐️ 6.0/10
2. [理解无法替代行动：用重复训练填补知行鸿沟](#item-tech-blog-2) ⭐️ 5.0/10
3. [十年慢性成瘾：如何放下大麻？](#item-tech-blog-3) ⭐️ 5.0/10

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [用 PowerShell 自定义 Windows 更新暂停时间](https://sspai.com/post/80562) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · 9月2日 07:22

**「背景」** Windows 10 及以后版本采用“软件即服务”模式，频繁推送更新，但系统界面最多只能暂停更新 35 天。对于需要长时间专注复杂项目的用户，这可能导致自动更新干扰工作，甚至丢失未保存的数据。作者因项目周期超过一个月，被迫寻找突破限制的方法。

**「方案」** 作者发现可以通过修改注册表来延长暂停时间。具体方法是：先在 Windows 更新设置中暂停更新，然后以管理员身份打开 PowerShell，执行一段脚本，将三个注册表项（PauseUpdatesExpiryTime、PauseFeatureUpdatesEndTime、PauseQualityUpdatesEndTime）的值设置为目标日期（如 2030-01-01）的 UTC 时间格式。脚本使用 Get-Date 解析日期，ToUniversalTime 转换时区，ToString 格式化，Set-ItemProperty 写入注册表。这样即可将暂停时间延长至任意日期，突破 35 天限制。作者还解释了 Windows 更新类型和企业延迟策略，但核心方法是这个注册表技巧。

**「启示」** 作者认为，虽然系统更新很重要，但在必要时可以通过注册表自定义暂停时间，延长 2-3 个月即可。完成工作后记得恢复更新，避免下次被强制更新打扰。

**标签**: `#Windows Update`, `#PowerShell`, `#Registry`, `#System Administration`, `#Productivity`

---

<a id="item-tech-blog-2"></a>
### [理解无法替代行动：用重复训练填补知行鸿沟](https://www.reddit.com/r/selfimprovement/comments/1w5eiy2/i_spent_two_years_knowing_exactly_what_was_wrong/) ⭐️ 5.0/10

reddit · r/selfimprovement · /u/Plus\_Ad3379 · 9月2日 16:02

**「背景」** 作者花了两年时间精确诊断自己的拖延问题，甚至能向他人清晰解释背后的心理机制，但生活却毫无改变。他意识到，理解问题本身成了一种舒适的避风港，让改变的紧迫感被搁置。

**「方案」** 作者指出，大脑存在两个系统：一个负责认知、计划和推理，另一个负责执行、启动和行动。前者可以通过阅读和研究无限发展，而后者只能通过实际行动来锻炼，尤其是当大脑倾向于选择轻松选项时，仍坚持做困难的事情。他尝试每周做一件没有外部目标的困难体力活动，不设追踪或观众，纯粹为了在低风险情境中练习克服不适感。起初几周毫无变化，但到第四或第五周，他开始感到对启动任务的阻力减弱，仿佛那个反对的声音仍在，但已不再自动服从。他总结道，行动系统需要的是重复练习，而非更多信息。

**「启示」** 作者的核心观点是，理解永远无法替代行动，过度分析反而可能成为停滞的借口。真正的改变来自通过重复执行困难任务来训练行动系统，而不是追求更完美的认知。

**标签**: `#knowing-doing gap`, `#self-improvement`, `#behavior change`, `#personal insight`, `#action vs understanding`

---

<a id="item-tech-blog-3"></a>
### [十年慢性成瘾：如何放下大麻？](https://www.reddit.com/r/selfimprovement/comments/1w5p7b8/chronically_high_for_almost_10_years_how_do_i_put/) ⭐️ 5.0/10

reddit · r/selfimprovement · /u/mia-bean · 9月2日 22:22

**「背景」** 作者从 19 岁开始使用大麻，并在两三个月内发展为每日使用，持续近十年。尽管表面上功能正常（大学荣誉毕业、稳定工作、研究生 GPA 4.0），但内心深感失控，多次尝试戒断均告失败。作者被诊断为 ADHD 和持续性抑郁障碍，但怀疑这些症状更多源于大麻使用障碍，而非独立的精神疾病。

**「方案」** 作者详细描述了成瘾的机制与挣扎：偏爱 THC 电子烟，因其廉价、无味且能带来强烈的“击中大脑”的快感，导致耐受性极高（100mg 食用品几乎无效）。戒断时最难的不是生理戒断症状，而是对那种感觉的渴求。曾改用花草和食用品六个月，但因找到旧烟弹而复发。作者还指出，大麻使用导致“动机缺乏综合征”，使日常任务变得异常困难，并可能被误诊为抑郁。此外，作者开始用酒精补偿大麻效果减弱，形成交叉成瘾风险。家庭成瘾史、创伤、跨性别身份、经济压力等加剧了困境。作者在治疗中，但尚未找到替代习惯或应对策略。

**「启示」** 作者的核心困境在于：大麻既是问题也是应对机制，戒断需要同时处理成瘾和填补情感空洞，但作者尚未找到可行的路径。这一叙述揭示了慢性大麻使用对动机、情绪和生活的深层影响，以及戒断的复杂性。

**标签**: `#cannabis use disorder`, `#addiction`, `#mental health`, `#personal narrative`, `#self-improvement`

---