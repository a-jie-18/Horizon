---
layout: default
title: "Horizon Summary: 2026-09-23 (EN)"
date: 2026-09-23
lang: en
---

> From 29 items, 2 important content pieces were selected

---

**Technology Blog**
1. [Coast: A FIRE-Oriented Bookkeeping App Built via Vibe Coding](#item-tech-blog-1) ⭐️ 6.0/10
2. [A 2001 Sony VAIO PCG-SRX7 Retrospective](#item-tech-blog-2) ⭐️ 5.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Coast: A FIRE-Oriented Bookkeeping App Built via Vibe Coding](https://sspai.com/post/114479) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Sep 22, 06:39

**「Background」** After ten years of personal bookkeeping, the author found that existing apps recorded data faithfully but never answered the real question: what do you do with all those records? Despite AI advice that the bookkeeping market was saturated and user migration costs were high, he decided to build his own app around the FIRE \(Financial Independence, Retire Early\) concept, because his accumulated data produced no decisions, no goals, and no usable budget.

**「Solution」** His methodology boils down to &quot;record as little as possible&quot;: merge accounts \(five credit cards into one, WeChat and Alipay into a single &quot;WePay&quot; account\), consolidate recurring spending \(monthly transit top-ups, coffee cards, holiday red packets, travel\), and classify by whether spending can be cut rather than by type—so &quot;dining out&quot; is separable while &quot;lunch&quot; is not. Coast turns this into product design: a FIRE page showing time-to-retirement, a sensitivity slider for monthly spend and income, and large-purchase simulation as a cooling-off period; each transaction shows its cost in days of delayed retirement. Spending is split into fixed, necessary, flexible, and other categories, each mapped to a FIRE role, and custom categories must declare that role. Auto-budgeting uses medians rather than averages, references the same month last year, and can tighten the historical baseline by a percentage. Other features include price tracking for repeated purchases and configurable &quot;attached spending&quot; like tips and taxes. On the Vibe Coding side, the author stresses writing a design-spec document first, learning Git \(commit per feature, branch for tests\), starting fresh conversations to control token costs, batching roughly ten bugs at a time, cropping screenshots, and letting Claude write code while Codex generates images via task descriptions.

**「Takeaway」** The author&\#x27;s larger point is that ten years of bookkeeping experience became the design foundation for Coast, and Vibe Coding gave a non-technical person the ability to realize those ideas—though shipping the app is only the beginning, since operations and promotion are the harder, ongoing challenge.

**Tags**: `#personal-finance`, `#FIRE`, `#vibe-coding`, `#app-design`, `#AI-assisted-development`

---

<a id="item-tech-blog-2"></a>
### [A 2001 Sony VAIO PCG-SRX7 Retrospective](https://sspai.com/post/114551) ⭐️ 5.0/10

rss · 少数派 \(生活方式与效率\) · Sep 22, 08:11

**「Background」** In 2001, the benchmark for a portable business laptop was set by machines like IBM&\#x27;s ThinkPad X22, which paired a 12.1-inch 1024x768 display and a Pentium III-M with a weight of 1.6–1.7kg. Sony&\#x27;s answer, the VAIO PCG-SRX series launched in late 2001, aimed to keep the same class of performance while shrinking the body to roughly B5 paper size and about 1.26kg with battery.

**「Solution」** The author&\#x27;s unit, the high-end PCG-SRX7, carries a Pentium III-M 800MHz, 128MB RAM \(upgraded to 256MB\), a 30GB drive, a 10.4-inch 1024x768 screen, built-in 2.4GHz Wi-Fi and Bluetooth, and Windows XP. Sony fit this into the small chassis partly through a dedicated &quot;Cascade cooling unit&quot; using very thin heat pipes, and the author notes the keyboard, circular SmartPad touchpad, and translucent blue-violet palm rest that lets indicator LEDs glow through. Restoring it was the real work: the BIOS cannot boot from USB and there is no internal optical drive, so Sony&\#x27;s original install path relied on an i.LINK \(IEEE 1394\) external drive; the author instead installed over ten drivers in a strict order from VAIOLibrary, since reversing the sequence leaves features inactive. Once complete, the Jog Dial worked system-wide for scrolling, menu selection, and Fn-based volume and brightness control. Networking proved the hard limit: the 2001 card supports only 802.11b with WEP, while modern routers use WPA2/WPA3 and disable legacy fallback, so the built-in Wi-Fi cannot connect; the practical fix is the RJ45 port, with correct system time and updated root certificates. The author also reports surprisingly loud, slightly spacious speakers and that Office 2003 plus Windows Media Player ran without constant memory pressure at 256MB.

**「Takeaway」** The author frames the SRX7 as evidence that Sony once balanced thinness, style, and performance in a way that still impresses 25 years later, though the account is a single-unit, hands-on nostalgia piece rather than a measured engineering analysis.

**Tags**: `#retro-computing`, `#laptop-hardware`, `#sony-vaio`, `#driver-compatibility`, `#nostalgia`

---