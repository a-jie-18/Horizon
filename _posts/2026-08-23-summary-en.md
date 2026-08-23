---
layout: default
title: "Horizon Summary: 2026-08-23 (EN)"
date: 2026-08-23
lang: en
---

> From 34 items, 4 important content pieces were selected

---

**Technology Blog**
1. [Reviving a Surface Pro 7 as a Linux AI Dashboard](#item-tech-blog-1) ⭐️ 7.0/10
2. [WinAirCast: Bridging Windows and HomePod with Low-Latency AirPlay 2](#item-tech-blog-2) ⭐️ 4.0/10
3. [The \#1 Skill for Better Conversations](#item-tech-blog-3) ⭐️ 4.0/10
4. [Going Smartphone-Free: Tips and Tradeoffs](#item-tech-blog-4) ⭐️ 4.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Reviving a Surface Pro 7 as a Linux AI Dashboard](https://sspai.com/prime/story/surface-pro-7-linux-ai-dashboard) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · Aug 23, 07:25

**「Background」** The author had a Surface Pro 7 that was nearly unusable under Windows 11 due to overheating and screen flickering during long sessions. Inspired by e-ink dashboards, they decided to repurpose the device as a desk-side AI usage dashboard and lightweight workstation, running Linux.

**「Solution」** The author used AI assistance throughout the process. They first discussed hardware and goals with an AI, which recommended Ubuntu 24.04 LTS, full disk wipe, LUKS encryption, and the linux-surface kernel for touch and pen support. Before rebooting, they had the AI generate a handoff prompt to continue guidance on their phone during installation. After booting into Ubuntu, they used a terminal agent to install the linux-surface kernel \(version 6.19.8-surface-3\) and troubleshoot issues: MOK signing for Secure Boot and GRUB boot order. They also solved the problem of booting without a keyboard by setting up TPM2-based auto-unlock with Clevis, binding to PCR 7. The final setup runs an AI usage dashboard and serves as a secondary screen for casual browsing.

**「Takeaway」** The author demonstrates that with AI assistance, a seemingly obsolete device can be transformed into a useful tool, and that Linux can breathe new life into hardware that struggles with modern operating systems.

**Tags**: `#Linux on Surface`, `#AI-assisted sysadmin`, `#TPM2 disk encryption`, `#linux-surface kernel`, `#hardware repurposing`

---

<a id="item-tech-blog-2"></a>
### [WinAirCast: Bridging Windows and HomePod with Low-Latency AirPlay 2](https://sspai.com/post/113002) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · Aug 23, 03:00

**「Background」** Windows users who want to stream audio to a HomePod face a common pain point: Windows lacks native AirPlay support. Existing third-party tools like TuneBlade and AirParrot often suffer from high latency, poor compatibility with modern Windows systems, and limited support for AirPlay 2 devices, making them unreliable for video sync and multi-speaker setups.

**「Solution」** The author introduces WinAirCast, a tool built from scratch in Rust that natively supports AirPlay 2 while remaining backward-compatible with AirPlay 1. It leverages AirPlay 2&\#x27;s PTP \(Precision Time Protocol\) for microsecond-level clock synchronization, enabling stable connections and synchronized playback across multiple speakers. WinAirCast offers a centralized device list, a desktop floating window, and a device dock that integrates with Windows 11&\#x27;s Fluent Design. Users can configure per-device streaming parameters, with a &\#x27;real-time streaming&\#x27; mode that reduces latency to as low as 45ms, and choose between ALAC \(lossless\) and PCM \(uncompressed\) encoding. The software also integrates Windows MMCSS Pro Audio scheduling to prioritize streaming threads and prevent audio glitches under heavy load. Additional features include a 10-band graphic equalizer with presets, flexible audio capture options \(global, per-app, or virtual audio devices for DRM-protected content\), and automatic standby when playback stops. The author provides a comparison table highlighting WinAirCast&\#x27;s advantages over TuneBlade and AirParrot, such as lower latency, better system compatibility, and more features, but these claims are promotional and lack independent benchmarks.

**「Takeaway」** The author&\#x27;s core thesis is that WinAirCast offers a modern, low-latency, and stable solution for streaming Windows audio to HomePod and other AirPlay devices, breaking down ecosystem barriers. The article serves primarily as a product announcement, emphasizing the tool&\#x27;s technical innovations and user-friendly design, but it does not provide independent verification of its performance claims.

**Tags**: `#AirPlay`, `#Windows`, `#audio streaming`, `#HomePod`, `#product announcement`

---

<a id="item-tech-blog-3"></a>
### [The \#1 Skill for Better Conversations](https://www.reddit.com/r/selfimprovement/comments/1vw8dls/this_is_the_1_skill_you_can_learn_for_conversions/) ⭐️ 4.0/10

reddit · r/selfimprovement · /u/yaboythewiseman · Aug 23, 14:17

**「Background」** As a nurse who meets four new patients daily, the author has learned to hold conversations with strangers despite being autistic. Interns often ask how he does it, prompting him to share his core technique.

**「Solution」** The author&\#x27;s advice is simple: people care less about what you say and more about whether you care about what they do. To engage someone, find something you&\#x27;re genuinely curious about and ask them about it, then listen without interrupting. He illustrates this with his own habit of asking about family to uncover love stories, then following up with questions about how they met, the proposal, and the wedding. Because he is genuinely excited, the other person becomes engaged and talks freely. He emphasizes that even if you&\#x27;re not naturally articulate, being curious and letting the other person talk can make a good impression. Once this basic skill is mastered, he suggests stacking more advanced techniques like establishing similarities and practicing deeper listening.

**「Takeaway」** The author&\#x27;s core thesis is that genuine curiosity and attentive listening are the most effective tools for holding conversations, even for those who struggle socially. This simple approach can transform interactions by making the other person feel valued.

**Tags**: `#conversation`, `#communication`, `#nursing`, `#anecdotal`, `#self-improvement`

---

<a id="item-tech-blog-4"></a>
### [Going Smartphone-Free: Tips and Tradeoffs](https://www.reddit.com/r/selfimprovement/comments/1vwit6n/going_smartphone_free_tips/) ⭐️ 4.0/10

reddit · r/selfimprovement · /u/the\_noobcat · Aug 23, 20:58

**「Background」** The author has been trying to go fully offline but realizes it&\#x27;s unrealistic due to work, social life, and daily needs. They&\#x27;ve managed to deactivate social media for months at a time but keep returning due to FOMO, birthday reminders, loneliness, and the habit of documenting life. Now they want to ditch the smartphone but are held back by essential features like NFC payments, GPS, health tracking, and messaging apps.

**「Solution」** The author proposes a realistic middle ground: limited screen time, a dumb phone, a LAN-based computer room, and keeping only forums like Reddit. They&\#x27;ve already brainstormed replacements for social media, such as direct photo sharing and calendar alerts. For the smartphone, they list must-have functions—NFC payments, navigation, health and period tracking, WhatsApp/Viber, music, photos, and taxi booking—and ask for advice on how to replicate these without a smartphone. They suggest possible workarounds like using a non-connected smartphone for photos, PC apps for messaging, and offline music, but seek community tips for a successful transition.

**「Takeaway」** The author&\#x27;s core challenge is balancing digital minimalism with practical needs, and they believe a hybrid approach—not full offline—is the only sustainable path. They invite others to share proven strategies for replacing smartphone functions, indicating that a successful transition requires creative substitutes rather than complete abandonment.

**Tags**: `#digital minimalism`, `#dumb phone`, `#smartphone alternatives`, `#screen time`, `#personal productivity`

---