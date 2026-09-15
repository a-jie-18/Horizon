---
layout: default
title: "Horizon Summary: 2026-09-15 (EN)"
date: 2026-09-15
lang: en
---

> From 44 items, 3 important content pieces were selected

---

**Technology Blog**
1. [AI-Assisted Excel Workflows: A Hands-On Comparative Test](#item-tech-blog-1) ⭐️ 7.0/10
2. [Photo Authenticity: Signatures, Depth, and Apple ARI](#item-tech-blog-2) ⭐️ 7.0/10
3. [派评：HomeKit 控制屏、自适应深色模式与本地语音工具](#item-tech-blog-3) ⭐️ 4.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [AI-Assisted Excel Workflows: A Hands-On Comparative Test](https://sspai.com/prime/story/ai-assisted-spreadsheeting-a-survey) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · Sep 14, 08:35

**「Background」** Since agentic AI took off, the author has wanted to drive a computer—or at least a spreadsheet—with natural language, but Microsoft&\#x27;s Office Copilot Pro left them unimpressed by its instruction-following and Office skills. With models and plugins improving fast, they set out to test what actually determines the quality of AI-assisted Excel deliverables in daily office work.

**「Solution」** The author built a structured comparison across models and &quot;harnesses&quot;—the way a model is invoked, with its own tools, APIs, environment, and rules. These ranged from Office sidebar add-ins \(OpenAI&\#x27;s and Anthropic&\#x27;s official plugins, plus the open-source Pi for Excel, which also runs Python snippets\) to standalone workbenches like Codex and Claude Cowork that take a file plus prompt end-to-end. Tests covered data cleaning, formula writing, and full deliverables, run in fresh files with reasoning set to high, tracking accuracy, hardcoding \(static values written instead of native dynamic formulas\), lossless handling of original data, and the number of human interventions needed. Formula writing proved mature, but complex workflows did not: on two pivot-table tasks, 16 of 22 outputs \(73%\) created a pivot table and 14 referenced the right source range, yet only 6 \(27%\) computed correctly, and sorting pivot tables defeated several models. On ambiguous data, most products silently decided for the user—XLOOKUP defaulting to the first match, or Workbuddy inventing names for unmatched records—even when the prompt said to stop and ask; Claude Cowork was the notable exception. Long, complex tasks required human intervention in 51% of 45 runs versus 12% for short basic tasks, with delays from overthinking, stalls \(a 10-minute LibreOffice residue hang, a 40-minute dead end\), and harness token limits. Harness mattered as much as model: with the same Claude model, the Excel add-in used modern XLOOKUP/FILTER/SORT, while Cowork fell back to VLOOKUP or INDEX+MATCH and hardcoded more, likely because it relies on LibreOffice, which lags on new Excel functions. The author&\#x27;s practical lessons: write rigorous prompts, tell the AI to ask when ambiguous, watch for black-box decisions, and after delivery change one raw value to check whether calculated cells update.

**「Takeaway」** The author concludes that AI is already strong at writing formulas, but reliable Excel delivery depends as much on the harness and prompt rigor as on the model, and that Office sidebar add-ins currently outperform standalone workbenches for spreadsheet work.

**Tags**: `#AI-assisted spreadsheets`, `#Excel automation`, `#LLM agents`, `#tooling evaluation`, `#prompt engineering`

---

<a id="item-tech-blog-2"></a>
### [Photo Authenticity: Signatures, Depth, and Apple ARI](https://sspai.com/post/114453) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · Sep 14, 07:16

**「Background」** As AI-generated and edited images spread, Apple&\#x27;s new Apple Reference Image \(ARI\) aims to prove a photo came from a real capture process rather than manipulation. Developer HaroldLee, who built the camera app TAPCam, argues the problem should be split into three questions: whether the file was modified, whether the capture pipeline is trustworthy, and whether the object in front of the lens is actually real.

**「Solution」** Digital signatures and secure hardware, the author explains, mainly address the first two questions. Based on public information and his own development experience—he cautions he has not obtained the iPhone 18 Pro or its APIs—he speculates ARI may sign sensor data at capture, then process it through Private Cloud Compute to produce a &quot;digital negative&quot; that binds the image to a trusted device and detects later tampering, similar in spirit to C2PA. But he stresses that a valid signature only proves a trusted camera took the photo; it cannot prove the subject was real, since a seller could photograph a badge displayed on a screen or printed on paper. His proposed extra layer is depth data: a genuine badge should have thickness and 3D structure, while screens and prints are largely flat, so combining image and depth could expose planar fakes. He acknowledges limits—depth may fail at distance or for very thin objects, and a physical counterfeit could still pass—so depth only raises the cost of forgery rather than guaranteeing truth. TAPCam instead uses Apple&\#x27;s App Attest, with a Secure Enclave–protected credential signing image and depth data, and verification performed in the browser to limit centralized data handling; the author notes ARI may upload photos to PCC, though hashing and signing in secure hardware could theoretically avoid that. He also suggests ARI&\#x27;s sensor-to-cloud channel might resist jailbroken devices better than app-layer APIs, but treats this as speculation.

**「Takeaway」** The author&\#x27;s core point is that signatures and secure capture can prove a photo came from a trusted process, but they cannot prove the thing photographed was real; depth data can only make faking harder. He argues image authenticity deserves to be a basic capability, not one reserved for expensive devices and complex services.

**Tags**: `#照片真实性`, `#数字签名`, `#C2PA`, `#深度数据`, `#iOS 安全`

---

<a id="item-tech-blog-3"></a>
### [派评：HomeKit 控制屏、自适应深色模式与本地语音工具](https://sspai.com/post/114577) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · Sep 14, 09:24

**「Background」** 本期《派评》汇总了多款近期值得关注的 App，覆盖智能家居、Android 自动化、本地 AI 语音、跨设备音频与 iOS 摄影等场景。这些工具大多针对系统自带功能未能满足的小众需求，例如把 iPad 变成固定的 HomeKit 控制屏、让手机根据环境光自动切换深浅色模式，或在无网络环境下完成语音转录。

**「Solution」** Dashboard 把 Apple Home 设备、摄像头、天气和日历重组成可自由拖拽、缩放的磁贴，iPad 支持分页、iPhone 为单页滚动，并允许隐藏磁贴；它还能接入未加入 HomeKit 的 RTSP 摄像头，支持 H.264 与新增的 H.265 流，兼容海康威视、大华、Reolink、Axis 等设备，并通过局域网搜索和 ONVIF 自动寻找视频流地址。免费版限制添加约 2～4 个设备，Premium 为 9.99 美元/年，解锁 3D 户型图、灯光高级控制和配置备份，含 7 天试用。Adaptive Theme 则利用 WRITE\_SECURE\_SETTINGS 权限，在每次亮屏时读取环境亮度并决定深浅色模式，授权方式包括 root、Shizuku、网络 ADB 或自建网络授权工具；它提供六个默认亮度阈值、自定义阈值、夜间模式保持、深浅色独立壁纸与锁屏模糊，作者实测自动换壁纸在亮屏后有一两秒延迟。Voxt 面向 macOS，既支持填入 Token 调用远程大模型，也支持本地模型完成转录、翻译和改写，通过 Fn、Fn+Shift、Fn+Control 触发，并针对 Apple Silicon 优化。MicYou 把 Android 手机变成电脑的虚拟麦克风，支持 Wi-Fi 局域网、USB 有线以及扫码即用的 Web 模式，内置 AI 降噪、混响、回声抑制、自动增益和均衡器，并可查看电平、延迟与丢包；作者实测 AI 降噪能明显减弱机箱风扇噪声，但受手机硬件限制，音质仍不及专业麦克风。Moment Pro Camera II 在 1.3 至 1.3.4 更新中加入慢快门（光轨与动态模糊、Bulb 模式）、更高等级防抖、假色、对焦放大镜、24MP 镜头支持以及 Action Plates 界面定制，售价 9.9 美元且无订阅。X Progress 7.0 新增照片主题工作室，可自定义背景、文字与指示器，自动抠出主体并添加动画，进度支持天数或百分比、剩余或已过方向，时间设置细化到分钟，提醒支持多次与重复，并可通过 iCloud 共享事件编辑；内购为 1.99 元/月、19.9 元/年或 148 元买断。

**「Takeaway」** 这些 App 的共同价值在于用相对轻量的方式补足系统能力的空白：把闲置设备变成专用控制屏、让模式切换真正跟随环境光、把语音处理留在本地，或让手机临时充当可用麦克风。作者认为，在厂商原生方案跟进之前，这类工具值得作为日常备选。

**Tags**: `#app-review`, `#roundup`, `#homekit`, `#android-automation`, `#local-ai`

---