---
layout: default
title: "Horizon Summary: 2026-08-24 (EN)"
date: 2026-08-24
lang: en
---

> From 34 items, 4 important content pieces were selected

---

**Technology Blog**
1. [AI-Powered Smart Standing Desk Conversion](#item-tech-blog-1) ⭐️ 8.0/10
2. [Making Windows on ARM Apps Native: A Practical Guide](#item-tech-blog-2) ⭐️ 7.0/10
3. [App Roundup: Motrix 2.0, WebToApp, Algidy, and More](#item-tech-blog-3) ⭐️ 6.0/10
4. [Per-App Volume Control on iPhone via Shortcuts](#item-tech-blog-4) ⭐️ 6.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [AI-Powered Smart Standing Desk Conversion](https://sspai.com/post/113563) ⭐️ 8.0/10

rss · 少数派 \(生活方式与效率\) · Aug 24, 07:14

**「Background」** The author, suffering from mild lumbar disc herniation, decided to upgrade his non-smart standing desk to support smart control. The original control panel lacked a child lock and obstacle detection, posing safety risks. Existing open-source solutions like Upsy Desky were incompatible with his desk&\#x27;s protocol, so he had to reverse-engineer the communication between the panel and control box.

**「Solution」** The author reverse-engineered the I²C protocol between the original panel and control box using a logic analyzer, discovering that the control box acts as the I²C master, polling the panel \(slave at address 0x24\) every ~3.7 ms for key codes. He identified key codes for up \(0x47\), down \(0x4F\), idle \(0x2E\), and presets. He then built an ESP32-S3 gateway that emulates the panel as an I²C slave, translating commands from multiple inputs \(Web, REST, BLE, keyboard, knob, voice\) into these key codes. A critical pitfall was missing pull-up resistors when replacing the panel, which he fixed by adding 2 kΩ resistors to the desk&\#x27;s 3.3V. He also attempted to read height data from the display channel \(addresses 0x34-0x37\) using software I²C, but it proved unstable, so he reverted to hardware I²C for key codes and added two ToF sensors for height and obstacle detection. The system includes a child lock, auto-away, and integration with Xiaozhi AI via MCP.

**「Takeaway」** The author demonstrates that with careful reverse engineering and iterative debugging, a non-smart standing desk can be transformed into a multi-device controlled smart desk, but stability requires using hardware I²C for critical communication and external sensors for height, rather than overcomplicating software emulation.

**Tags**: `#I2C protocol reverse engineering`, `#ESP32-S3`, `#standing desk automation`, `#embedded systems`, `#hardware hacking`

---

<a id="item-tech-blog-2"></a>
### [Making Windows on ARM Apps Native: A Practical Guide](https://sspai.com/prime/story/create-your-own-windows-apps) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · Aug 24, 08:28

**「Background」** Windows on ARM has matured significantly, but many apps still run via emulation, which incurs performance and power overhead. Since official ARM64 native versions are often unavailable, the author explores practical methods to convert common apps to run natively on ARM64.

**「Solution」** The author identifies two main approaches. First, for web-based services, they suggest using PWA installation or the open-source tool Pake to package web pages into standalone ARM64 native apps. Pake uses Tauri and WebView2, resulting in small, low-memory apps. The author provides steps to install Pake CLI locally and compile an app, noting that the official cloud workflow lacks ARM64 support. Second, for Electron-based apps, the author explains that these consist of a runtime shell \(Chromium + Node.js\) and an app.asar file containing cross-platform code. By replacing the x64 Electron shell with an ARM64 version and keeping the app.asar, the app can run natively. The author demonstrates this with the design tool 墨刀, detailing how to check the Electron version, download the ARM64 runtime, copy the app.asar, rename the executable, and restore the icon using Resource Hacker.

**「Takeaway」** The author concludes that many seemingly x86-only apps can be converted to run natively on Windows on ARM with minimal effort, improving performance and reducing resource usage. This approach empowers users to take control of their software environment without waiting for official support.

**Tags**: `#Windows on ARM`, `#Electron`, `#Pake`, `#ARM64`, `#app conversion`

---

<a id="item-tech-blog-3"></a>
### [App Roundup: Motrix 2.0, WebToApp, Algidy, and More](https://sspai.com/post/113795) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Aug 24, 09:52

**「Background」** In this roundup, the author reviews six apps that address common productivity gaps, from downloading files to managing food expiry and remote AI agents. Each app offers a practical solution to a specific pain point, but the reviews are mostly feature lists with limited depth.

**「Solution」** The author highlights Motrix 2.0, a download manager rebuilt from scratch with a headless server for NAS deployment and CLI support for AI agents. WebToApp lets Android users turn websites into standalone APKs locally, with support for scripts and extensions. Algidy tracks food expiry via barcode scanning, while 不空 provides fishing weather and catch records. Moshi enables mobile control of AI agents on Mac/Linux, though it requires Tailscale for remote access. Capture serves as a universal inbox for Apple users, routing content to various apps with format-specific exports.

**「Takeaway」** The author concludes that these apps offer incremental improvements for specific tasks, but none provide groundbreaking innovation. They are useful for users with matching needs, but the reviews lack comparative analysis or transferable insights.

**Tags**: `#app reviews`, `#productivity`, `#download manager`, `#AI agent`, `#mobile apps`

---

<a id="item-tech-blog-4"></a>
### [Per-App Volume Control on iPhone via Shortcuts](https://sspai.com/post/112983) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Aug 24, 03:30

**「Background」** Many Android phones allow setting independent volumes for different apps, but iOS lacks this feature. Users may want quieter short-video apps, louder video apps, or lower volume for bedtime listening. The author proposes a workaround using Shortcuts automations.

**「Solution」** The solution uses two automations: when opening an app, save the current media volume and the app name, then set the volume to the saved value for that app. When closing the app, save the current volume \(if adjusted\) and restore the original volume. This relies on iOS 27&\#x27;s new storage feature in Shortcuts, which allows persistent data storage with global values, enabling the automations to share data. For older iOS versions, the author provides a file-based alternative that mimics the same logic. A critical setting is to disable &\#x27;Change with Buttons&\#x27; in Sound &amp; Haptics, because Shortcuts&\#x27; &\#x27;Get Device Details&\#x27; only retrieves ringtone volume when that is enabled, not media volume. Limitations include the first launch volume resetting to zero and a volume HUD appearing on each adjustment.

**「Takeaway」** The author demonstrates that with iOS 27&\#x27;s storage feature, Shortcuts can effectively implement per-app volume control, offering a practical workaround for a missing system feature, though it requires careful setup and has minor UX tradeoffs.

**Tags**: `#iOS Shortcuts`, `#automation`, `#volume control`, `#iPhone`, `#workflow`

---