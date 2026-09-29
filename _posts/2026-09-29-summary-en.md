---
layout: default
title: "Horizon Summary: 2026-09-29 (EN)"
date: 2026-09-29
lang: en
---

> From 45 items, 2 important content pieces were selected

---

**Technology Blog**
1. [iPhone Duo&\#x27;s Interaction Design as Apple&\#x27;s Best Practice](#item-tech-blog-1) ⭐️ 7.0/10
2. [Running a Terminal AI Agent on Android via Termux](#item-tech-blog-2) ⭐️ 6.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [iPhone Duo&\#x27;s Interaction Design as Apple&\#x27;s Best Practice](https://sspai.com/post/114972) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · Sep 28, 07:00

**「Background」** Folding phones have long suffered from ad-hoc adaptation: apps are merely stretched or padded to fit the inner screen, and the interaction model inherited from ordinary smartphones has never been properly standardized. Microsoft&\#x27;s Surface Duo tried to map out usage postures but was dragged down by slow hardware and Android&\#x27;s fragmented ecosystem, and it died after two generations. When Apple announced the iPhone Duo, the author&\#x27;s initial concern was the crease, but the promotional videos made the interaction design the far more compelling story.

**「Solution」** The author traces Apple&\#x27;s approach back to the 1987 Human Interface Guidelines, whose first chapter insists that people are trying to get their jobs done, not use computers, and to designer Chan Karunamuni&\#x27;s WWDC talks. In 2018&\#x27;s Designing Fluid Interfaces, Chan argued that interfaces must respond to people&\#x27;s changing actions, not the reverse; in 2023 he showed how Dynamic Island&\#x27;s expanded view preserves the relative placement of elements so users keep their bearings; in 2025 he framed Liquid Glass as the accumulation of lessons from Aqua, iOS 7, iPhone X, Dynamic Island, and visionOS. From these, the author derives six &quot;meta design principles&quot;—context first, controllable process, spatial continuity, task continuity, clear feedback, and experience transfer—and applies them to the Duo. The device is organized around a &quot;book&quot; metaphor, used explicitly in Apple&\#x27;s Design for iPhone Duo talk: it can be used partially folded like a book. This explains the side-mounted Dock and toolbars, which keep controls near the thumb and aligned with the camera across folding states, and the hinge-angle-driven unfolding animation, where blur gradually resolves into a sharp lock screen as the device opens. Adaptive layouts move popovers and paired components away from the crease, while scrollable content is left to scroll past it. The author flags that the bookmark analogy and the exact rendering algorithm behind the unfolding effect are his own inferences, not documented facts.

**「Takeaway」** The author&\#x27;s core thesis is that Apple&\#x27;s Duo design is not a visual evolution but a sustained ability to re-ask foundational questions—returning to human intent, then rebuilding interaction from there. Whether the hardware succeeds will take a year to judge, but the design effort is already the more visible achievement.

**Tags**: `#interaction-design`, `#folding-devices`, `#Apple-HIG`, `#WWDC`, `#UI-adaptation`

---

<a id="item-tech-blog-2"></a>
### [Running a Terminal AI Agent on Android via Termux](https://sspai.com/prime/story/dev-env-on-android-with-termux) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Sep 28, 09:33

**「Background」** Terminal AI agents like Hermes and Pi differ from web chat boxes in that they can run scripts, edit code, and debug directly in the command line, making them genuine working assistants. The author argues the most convenient always-available device for such an agent is the phone you already carry, since a computer isn&\#x27;t always at hand and renting a cloud server costs extra, while an Android phone has network, power, and enough performance for a modern Linux CLI environment. The main obstacles on Android are the system&\#x27;s aggressive background process killing and low-level compatibility issues some CLI tools have on the platform.

**「Solution」** The author&\#x27;s setup, tested on a Xiaomi 15 Ultra without root or flashing, starts by installing Termux from GitHub Releases rather than an app store, because the Play Store version is unmaintained and F-Droid&\#x27;s signing key differs from GitHub&\#x27;s, which breaks later plugin installs; the termux-api and termux-boot plugins are installed alongside. After granting storage permission, switching to a domestic mirror, and upgrading packages, the author installs Python and build dependencies, clones Hermes Agent, and installs it with the \[termux\] extra to avoid incompatible desktop dependencies. Hermes then bootstraps its own configuration interactively \(the author chose DeepSeek for cheap pay-as-you-go pricing\) and installs the rest of the toolchain on request. A compatibility table lists Hermes and Pi as natively supported, OpenCode, Codex CLI, Grok Build, and Cursor CLI as needing community forks, source builds, or a proot Ubuntu container, and Claude Code as having no stable solution. For keepalive, the author recommends three layers: setting the battery policy to unrestricted, disabling lock-screen memory cleanup, and enabling &quot;Disable child process restrictions&quot; in developer options to counter Android&\#x27;s Phantom Process Killer. As a fallback, the author exploits Android&\#x27;s background exemption for media playback by looping a one-minute silent WAV generated with ffmpeg, but notes this can seize the A2DP Bluetooth channel and cut out headphones, so the keepalive script should detect a Bluetooth connection and pause playback until it disconnects. The source is truncated mid-script, leaving the keepalive solution incomplete.

**「Takeaway」** The author&\#x27;s core point is that a non-rooted Android phone running Termux can serve as a genuinely usable portable server for terminal AI agents and light development, provided you install Termux from the right source and defeat Android&\#x27;s process-killing behavior with layered settings and a Bluetooth-aware silent-audio keepalive. The evidence is anecdotal, from a single device, and the compatibility table is unsourced and dated to 2026, so readers attempting this exact setup should treat the details as a starting point rather than verified fact.

**Tags**: `#Termux`, `#Android`, `#CLI AI agents`, `#mobile dev environment`, `#process keepalive`

---