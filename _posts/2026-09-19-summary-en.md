---
layout: default
title: "Horizon Summary: 2026-09-19 (EN)"
date: 2026-09-19
lang: en
---

> From 38 items, 2 important content pieces were selected

---

**Technology Blog**
1. [Getting Personal Health Data Into AI Agents: Seven Paths](#item-tech-blog-1) ⭐️ 7.0/10
2. [watchOS 27 Hands-On: Dynamic App Grid and Smarter Stacks](#item-tech-blog-2) ⭐️ 4.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Getting Personal Health Data Into AI Agents: Seven Paths](https://sspai.com/prime/story/how-to-obtain-data-for-agent-analysis) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · Sep 18, 03:19

**「Background」** The author hit a training plateau and wanted an AI agent to help diagnose it, which raised a prior question: how can an agent continuously obtain health data the author already records? The article is the first in a series and addresses only that acquisition problem, acknowledging that hands-on testing covered Apple Health and Oura while other vendors&\#x27; details come from public sources.

**「Solution」** The author frames health data as three layers—raw records like steps and heart rate; algorithm-derived metrics like readiness, strain, and resilience; and manual entries such as diet and training feel—spread across aggregator platforms \(Apple Health, Health Connect, Google Health\), vendor or specialist apps \(Oura, Whoop, Garmin, Hevy\), and reports with no stable digital entry. Vendors sync some but not all of this to aggregators, since platforms may lack matching fields and composite metrics are subscription selling points, so the first question is whether the needed data already reaches an aggregator and whether its fields suffice. Seven paths follow: using AI products&\#x27; built-in Apple Health access \(region- and account-gated, best for light queries\); ready-made connectors or relay services like Strava&\#x27;s MCP connector, Xunji&\#x27;s API Skill, Hevy&\#x27;s API key, and Freddy, at the cost of third-party storage; continuous export from aggregators, where Apple Health supports Shortcuts, paid tools like Health Push and Health Auto Export, or a self-built app via an open SDK, while Android&\#x27;s Health Connect offers Health Sync and Health Data Export; and direct vendor APIs or SDKs, including Google Health&\#x27;s API and CLI, Oura and Whoop&\#x27;s OAuth developer apps, Samsung&\#x27;s Data SDK, and China&\#x27;s vendor platforms, where only Huawei&\#x27;s Health Service Kit appears open to individuals. Practical caveats include OAuth token refresh and persistence, incremental sync with dedup keys and resumable checkpoints, WHOOP&\#x27;s physiological-cycle unit rather than calendar days, and deprecated Oura PAT and old WHOOP webhooks that break older tutorials.

**「Takeaway」** The author&\#x27;s core point is that choosing a data path should start from where the data already lives and whether the aggregator&\#x27;s fields are sufficient, not from the flashiest integration; convenience usually trades against control, and long-term accumulation favors storing data where you can export and query it yourself.

**Tags**: `#health-data`, `#ai-agents`, `#apple-health`, `#api-integration`, `#personal-data`

---

<a id="item-tech-blog-2"></a>
### [watchOS 27 Hands-On: Dynamic App Grid and Smarter Stacks](https://sspai.com/post/114670) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · Sep 18, 03:30

**「Background」** Apple released watchOS 27 on September 15 alongside iOS 27, iPadOS 27, and macOS 27 Golden Gate, but the update only supports Apple Watch Series 9 \(2023\) and later, paired with an iPhone 11 or newer running iOS 27. A hands-on roundup from 少数派编辑部 walks through what changed, mixing brief first-hand impressions with features restated from Apple&\#x27;s marketing and release notes.

**「Solution」** The author&\#x27;s main hands-on observations center on three areas. Liquid Glass, introduced in watchOS 26, now has what Apple calls more uniform refraction and improved contrast; in use, buttons feel deeper and more three-dimensional, light backgrounds gain contrast, and glass controls blur more heavily so background content barely shows through. Notably, iOS&\#x27;s Liquid Glass intensity slider does not come to watchOS, so the effect is fixed near iOS&\#x27;s default level. Pressing the Digital Crown now opens a Dynamic app grid that blends the app grid with Siri suggestions, placing frequently used apps and recommendations more prominently; the author found the larger icons easier to tap on a small screen, and users can still switch to the traditional grid. Smart Stack also becomes more proactive, surfacing widgets based on time, location, and context—birthdays, parked-car navigation, holiday alarms, transit cards, upcoming calendar items, rain forecasts, frequent iMessage contacts, and post-workout summaries. A new single-finger double-tap gesture opens the selected Smart Stack widget, with a silver highlight ring indicating selection; unlike the two-finger double-tap used for paging in Settings or the app grid, this gesture only works within Smart Stack. The Find app consolidates Find Devices, Find Contacts, and Find Items into one map-based app with Precision Finding for iPhone, second-generation AirTag, and AirPods Pro 3. The author also notes forward-looking Siri AI features that are unavailable in their region, plus smaller changes: perimenopause and menopause tracking, revised Apple Watch For Your Kids setup, faster Apple Music launch, synced step counts, improved indoor distance tracking, battery optimization suggestions, water-detection algorithm upgrades, Wi-Fi improvements, faster widget and complication launches, a redesigned Watch app settings page, time-zone-aware Sleep mode, a Siri module watch face, and Wallet guest keys. Several claims—page-load performance, touch response, battery life, and water detection—are described from subjective feel or unspecified fields rather than measured evidence.

**「Takeaway」** The author concludes that watchOS 27 is an unremarkable but genuinely useful update, pairing a few practical new features with performance and battery improvements, while its most contentious point is dropping support for Apple Watches older than Series 9.

**Tags**: `#watchOS`, `#Apple Watch`, `#wearables`, `#feature roundup`, `#user experience`

---