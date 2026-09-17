---
layout: default
title: "Horizon Summary: 2026-09-17 (EN)"
date: 2026-09-17
lang: en
---

> From 38 items, 2 important content pieces were selected

---

**Technology Blog**
1. [Remembering EdgeHTML: What Old Edge Got Right](#item-tech-blog-1) ⭐️ 6.0/10
2. [iPadOS 27: Liquid Glass Tweaks, Speed, and AI](#item-tech-blog-2) ⭐️ 4.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Remembering EdgeHTML: What Old Edge Got Right](https://sspai.com/post/113295) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Sep 16, 02:38

**「Background」** Microsoft&\#x27;s EdgeHTML-based Edge, launched with Windows 10 in 2015, was retired and stopped receiving support on March 9, 2021, later replaced by the Chromium-based Edge. The author, writing on the fifth anniversary of that end of support, revisits why the original browser was technically distinctive and why it ultimately failed.

**「Solution」** The author argues EdgeHTML&\#x27;s strengths came from deep integration with Windows: it used DirectComposition and Direct Manipulation for asynchronous, inertia-based smooth scrolling that he considers still unmatched, DirectWrite for font rendering closer to Windows defaults than Chromium&\#x27;s Skia \(a difference more visible in CJK text, later partly addressed by a Chromium patch after Chrome 132\), and native Windows components like Media Foundation and the WinRT PDF renderer, plus a reflowable, paginated EPUB reader with ink annotation. Microsoft also prioritized APIs used by real sites over standards-checklist completeness, using Bing crawl data to find compatibility gaps. But the same OS coupling was fatal: Edge shipped only on Windows 10 and its features arrived with semi-annual Windows updates, so enterprises that deferred upgrades fell behind, extension support came late, and low usage discouraged developers from testing against it. Building on the immature UWP platform further slowed iteration, and the team could not match Chrome&\#x27;s release pace. Microsoft therefore moved to Chromium, a decision the author calls commercially correct. He connects this to engine monoculture: when Chrome dropped Manifest V2 support in 2024, downstream Chromium browsers like Edge Chromium eventually had to follow, since preserving V2 would require forking and painful backporting; XSLT removal is a similar case. He notes Firefox and Safari remain compatibility targets but hold too little share.

**「Takeaway」** The author&\#x27;s nostalgia is less about a single browser than about what independent engines made possible: EdgeHTML&\#x27;s OS-tied design produced genuinely better scrolling, fonts, and reading, yet that same coupling and its small user base doomed it. Its death, and the later forced retreat on Manifest V2 and XSLT, illustrate how a Chromium monoculture lets one company&\#x27;s decisions propagate across nearly the whole web, with little users can do.

**Tags**: `#browser-engines`, `#edgehtml`, `#chromium-monoculture`, `#web-standards`, `#manifest-v2`

---

<a id="item-tech-blog-2"></a>
### [iPadOS 27: Liquid Glass Tweaks, Speed, and AI](https://sspai.com/post/114607) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · Sep 16, 07:00

**「Background」** Apple released iPadOS 27 alongside iOS 27, macOS 27 Golden Gate, and watchOS 27, continuing to refine the Liquid Glass design language introduced the previous year while touching performance, interaction, and AI. For readers deciding whether to upgrade, the question is what actually changed beyond cosmetic polish.

**「Solution」** The author&\#x27;s walkthrough frames iPadOS 27 as a round of detail-level adjustments rather than a major UI overhaul. Liquid Glass changes include edge-to-edge sidebars returning to the iPadOS 18 style \(which the author personally finds less dimensional than OS 26\), rebuilt system app icons, new light-and-shadow rendering for buttons, notifications, text fields, and context menus, and a transparency slider in Settings &gt; Appearance whose most opaque setting resembles iPadOS 18&\#x27;s frosted look. The menu bar now shows the app name at the top by default and reveals options on tap, reducing accidental gestures, partly because the top-center pull-down is reassigned to the new Siri AI; users can pin the menu bar instead. SF Symbols in menus were largely removed, matching macOS 27, leaving mainly window-control icons. Home screen edits gain undo/redo, iPhone app windows resize more freely, and Sidecar now supports multi-touch gestures like scrolling and pinch-to-zoom on the iPad screen. Apple Pencil gets a new charging sound, handwritten notes become Spotlight-indexable via PencilKit \(so third-party PencilKit apps benefit too\), and Notes can copy content as Markdown. Performance improvements are mostly described qualitatively, but the author&\#x27;s file-copy test is concrete: 3.74 GB from an SSD to an iPad mini&\#x27;s internal storage took about 5 seconds, and 21 GB from the iPad mini to the SSD took under 30 seconds, suggesting the 10 Gbps bandwidth is nearly saturated. On AI, Apple Foundation Models gain Google Gemini assistance while Apple says the models remain self-developed, adding agentic capabilities and system-level context and screen awareness; however, Apple Intelligence and Siri AI features remain unavailable on China-market iPads.

**「Takeaway」** The author&\#x27;s overall impression is that iPadOS 27 keeps polishing Liquid Glass while advancing performance, interaction, and features, and that Apple appears to be deliberately bringing macOS and iPadOS closer together. The piece is a changelog-style overview with limited benchmarks, so its performance and design judgments rest largely on the author&\#x27;s hands-on impressions.

**Tags**: `#iPadOS`, `#Apple`, `#UI design`, `#release notes`, `#consumer tech`

---