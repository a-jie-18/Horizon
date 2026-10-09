---
layout: default
title: "Horizon Summary: 2026-10-09 (EN)"
date: 2026-10-09
lang: en
---

> From 36 items, 3 important content pieces were selected

---

**Technology Blog**
1. [Mole: From Open-Source CLI to Paid Mac App](#item-tech-blog-1) ⭐️ 7.0/10
2. [A Designer&\#x27;s Critique of iPhone Duo&\#x27;s Asymmetric Layout](#item-tech-blog-2) ⭐️ 6.0/10
3. [A Room-by-Room Decluttering System Built Over Four Years](#item-tech-blog-3) ⭐️ 4.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Mole: From Open-Source CLI to Paid Mac App](https://sspai.com/post/113843) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · Oct 8, 08:10

**「Background」** Mole began as an open-source Mac cleaning CLI that the author wrote for himself and colleagues, then unexpectedly grew to 60K stars, 50+ releases, and 121 contributors. The recurring user request — from people whose relatives use Macs but can&\#x27;t open a terminal — pushed him to build a paid desktop version, while the CLI stayed free and open source.

**「Solution」** The core insight is that a cleaner&\#x27;s value lies less in how much it deletes than in letting users see clearly before anything is removed. The author sorts scanned items into three tiers: regenerable \(HTTP/GPU caches, build artifacts, most logs\), costly-to-rebuild \(package-manager caches, local model weights, iOS DeviceSupport\), and irreplaceable \(chat history, mail, photos, active project state\) — the last never entering a one-click list. AI coding tools amplified junk in three ways: build outputs \(one Rust target cleanup freed 86G\), auto-updated CLI tools leaving ~250MB old versions, and tens of GB of Ollama/LM Studio/HuggingFace models. Model paths like ~/.ollama/models and ~/.cache/huggingface are hard-coded protection lists because Ollama splits models into hash-named shared blocks that only the tool can safely dereference; AI session records \(~/.codex/sessions, ~/.claude/projects\) are never touched. These rules were learned the hard way — early CLI versions deleted com.apple.e5rt.e5bundlecache, breaking recognition features until reboot. macOS Install Data gets three gates \(pending update, recent modification, running processes\) plus a re-check at deletion time. The tradeoff is acknowledged: scanning and confirmation make it slower, but the author prefers missing deletions to wrong ones. User emails drove concrete changes — defaulting to Celsius, adding light-mode requests, and keeping manual email support \(refund rate under 0.8%\) rather than automating before problems, answers, and exceptions are stable.

**「Takeaway」** The author argues that deciding what not to do matters more than what to build, and that in an AI era where code barriers shrink, trust built through genuine user conversation is the product&\#x27;s longest-lived asset.

**Tags**: `#macOS`, `#developer-tools`, `#product-development`, `#AI-coding`, `#open-source`

---

<a id="item-tech-blog-2"></a>
### [A Designer&\#x27;s Critique of iPhone Duo&\#x27;s Asymmetric Layout](https://sspai.com/post/115282) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Oct 8, 09:28

**「Background」** Apple has a track record of reworking existing product categories on its own terms, so a designer who uses both foldables and iPhones expected the rumored iPhone Duo to set a new bar for foldable UX. After the launch and early media hands-ons, though, the author found the device less compelling than hoped and wrote a static, pre-sale critique of its design choices.

**「Solution」** The author&\#x27;s central argument is that hardware decisions appear to have driven software rationalization. To save vertical space on a short, D-shaped outer screen, Duo moves controls like back and toolbars into a vertical Control Area on the right, shrinking many buttons to icons and breaking the muscle-memory conventions iPhone users rely on; the author expects mis-taps and relearning costs, especially for third-party apps with custom icons. The space saving is also questionable: the author claims the folded Duo is about 1.16x wider than an iPhone 18 Pro but offers only about 0.94x the effective horizontal content width, because the control strip stays reserved even when few controls exist. The same separation undermines Liquid Glass, whose translucency depends on content behind it; moving glass controls onto blank side space removes that backdrop. The author speculates the asymmetry stems from hardware being locked before software design, then being given a bespoke interaction model to look intentional, much like the Dynamic Island. Multitasking is likewise conservative—only basic Split View, no outer-screen or vertical split, no ratio adjustment, and no Stage Manager or free-form windows. Two hardware details also draw scrutiny: the inner under-display camera is not truly hidden and might be better pushed to the edge, while the outer camera&\#x27;s right-side placement locks in the asymmetric layout; the author suggests a centered camera and symmetric outer screen as a more familiar alternative. Finally, Duo appears to be the first foldable with the charging port on the left half, so a plugged cable swings during opening and closing, clashing with the carefully polished digital transition animation.

**「Takeaway」** The author concludes that Duo shows genuine design novelty but leaves unresolved tensions: a hardware-first asymmetry that reshapes software, weakens Liquid Glass, and limits multitasking. Because the analysis is based on limited second-hand material and static inspection, the author frames it as a pre-sale discussion to be verified after hands-on use.

**Tags**: `#Apple`, `#product design`, `#UX`, `#foldables`, `#hardware-software integration`

---

<a id="item-tech-blog-3"></a>
### [A Room-by-Room Decluttering System Built Over Four Years](https://sspai.com/post/115209) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · Oct 8, 06:42

**「Background」** The author has decluttered roughly once a year for several years, and over time the practice evolved from ad-hoc purging into a standardized, room-by-room routine. The recurring problem she identifies is that homes are designed around past habits or imagined futures, so mismatches accumulate between how people actually live and how their space is laid out.

**「Solution」** Her central insight is that decluttering is less about emptying a house than about observing your own habits and then letting the placement of objects follow them. She splits the home into zones \(bedroom, bathroom, kitchen, wardrobe, storage room\) and assigns each a fixed slot on the calendar, spreading the whole job over about four months rather than one doomed weekend; the order matters because the storage room doubles as a holding area for undecided items, which are then judged months later by whether they were ever missed. General rules include: a necessity is something you would immediately repair or replace if broken; forgotten functional items \(a tamagoyaki pan, a pasta strainer\) can go; and low-maintenance materials are preferred to cut upkeep time. Two methods do the actual sorting: a two-box approach \(discard vs. pending\) for fast-judgment areas like the bedroom, and a single-box one-month test for high-frequency areas like the kitchen and bathroom, where everything is boxed and only what you retrieve in a month returns to its place. She also carves out a dedicated spot for &quot;mid-frequency&quot; items—things used often but not daily, such as worn-once clothes, hair ties, and bag clips—since these are what scatter and get repurchased; the rule of thumb is to store an item wherever you first instinctively looked for it. The final step is reviewing consumption: she traces purchases back to coupon-driven or impulse buys, argues that frequently used, long-lived items \(mattress, pressure cooker\) deserve the best you can afford while rarely used gadgets do not, and notes that repair or a cheap replacement part often rescues items that only seem like junk.

**「Takeaway」** The author&\#x27;s conclusion is that decluttering is not about achieving extreme emptiness but about regaining control of your space, and that the process doubles as a mirror for how your consumption and daily habits have shifted over the years. The evidence is entirely personal and anecdotal, so the heuristics are best read as one person&\#x27;s tested routine rather than a general prescription.

**Tags**: `#decluttering`, `#personal-productivity`, `#home-organization`, `#lifestyle`, `#anecdotal`

---