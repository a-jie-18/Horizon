---
layout: default
title: "Horizon Summary: 2026-09-09 (EN)"
date: 2026-09-09
lang: en
---

> From 43 items, 4 important content pieces were selected

---

**Technology Blog**
1. [The Seamless Secrets Behind Apple Sidecar&\#x27;s Smooth Experience](#item-tech-blog-1) ⭐️ 8.0/10
2. [Animated Windows 11 Avatar via Registry and PsExec](#item-tech-blog-2) ⭐️ 5.0/10
3. [A Summer Journey Through Kyushu and Amami Oshima](#item-tech-blog-3) ⭐️ 5.0/10
4. [Community Digest: NuPhy Keyboard and Anti-Algorithm Info Sources](#item-tech-blog-4) ⭐️ 4.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [The Seamless Secrets Behind Apple Sidecar&\#x27;s Smooth Experience](https://sspai.com/prime/story/sidecar-optimizations) ⭐️ 8.0/10

rss · 少数派 \(生活方式与效率\) · Sep 8, 10:14

**「Background」** Apple&\#x27;s Sidecar lets an iPad serve as a wireless secondary display for a Mac, but achieving a fluid, near-invisible experience is technically demanding. The author notes that while third-party solutions like iDisplay, Air Display, and Duet Display existed earlier, they suffered from lag, instability, or high CPU usage. Sidecar&\#x27;s advantage lies not in the virtual display concept but in the sophisticated pipeline that encodes, transmits, and decodes screen frames efficiently.

**「Solution」** The key to Sidecar&\#x27;s smoothness is its use of HEVC \(H.265\) video encoding to compress the screen stream before wireless transmission. Raw screen data is enormous—a 2388×1668 frame at 60Hz generates nearly 1 GB per second—so compression is essential. HEVC works by dividing frames into coding tree units \(CTUs\) and using intra-prediction \(from neighboring pixels within the same frame\) and inter-prediction \(from other frames\) to predict content, recording only residuals and motion vectors. The author demonstrates that HEVC can reduce a 363.2 MB video to about 2% of its size with near-visual-lossless quality. Sidecar leverages hardware-accelerated encoding and decoding on both Mac and iPad, minimizing latency. The article also explains frame types \(I, P, B\) and GOP structure, showing how the encoder balances efficiency and quality. While the author notes that current beta touch input is smooth, most apps still translate touches to mouse actions, and quantitative latency measurements are not provided.

**「Takeaway」** Sidecar&\#x27;s seamless experience stems from Apple&\#x27;s integration of efficient HEVC encoding and hardware acceleration, turning a complex wireless video streaming problem into a nearly imperceptible solution. This technical foundation, rather than the mere concept of using an iPad as a display, is what sets Sidecar apart from earlier third-party attempts.

**Tags**: `#Sidecar`, `#HEVC`, `#video encoding`, `#screen mirroring`, `#iPad as display`

---

<a id="item-tech-blog-2"></a>
### [Animated Windows 11 Avatar via Registry and PsExec](https://sspai.com/post/114312) ⭐️ 5.0/10

rss · 少数派 \(生活方式与效率\) · Sep 8, 07:00

**「Background」** Windows 11 does not natively support animated GIFs as user avatars; uploading one via settings results in a static image. The author, inspired by a tweet, explains that Windows actually supports GIF avatars but requires editing registry values under the AccountPicture key, which cannot be modified with standard permissions.

**「Solution」** To set an animated avatar, you must edit the registry as the SYSTEM account. The author recommends using PsExec from Microsoft&\#x27;s Sysinternals suite. After downloading and extracting PsTools, add its folder to the system PATH via Environment Variables. Then, launch an elevated terminal and run \`psexec -i -s regedit.exe\`, where \`-i\` enables an interactive interface and \`-s\` runs as SYSTEM. In the registry editor, navigate to \`HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\Windows\\CurrentVersion\\AccountPicture\\Users\\\` and change all avatar values to the file path of your GIF. The author notes that Windows 11 also supports transparent animated images, which can make the login screen more immersive. They emphasize backing up before proceeding.

**「Takeaway」** The author demonstrates that with system-level registry access, Windows 11 can display animated GIF avatars, offering a simple customization trick for users willing to follow the steps.

**Tags**: `#Windows 11`, `#registry`, `#GIF avatar`, `#PsExec`, `#customization`

---

<a id="item-tech-blog-3"></a>
### [A Summer Journey Through Kyushu and Amami Oshima](https://sspai.com/post/113299) ⭐️ 5.0/10

rss · 少数派 \(生活方式与效率\) · Sep 8, 03:06

**「Background」** The author, inspired by a friend&\#x27;s remark about the unexplored Amami Oshima, decides to travel there. Before meeting the friend, they spend a few days in Kyushu seeking out &\#x27;穴場&\#x27; \(hidden gems\) — lesser-known places worth a special trip. The narrative captures the appeal of spontaneous exploration and the desire to see what these overlooked spots have to offer.

**「Solution」** The author&\#x27;s approach is to wander without rigid plans, using maps and curiosity to discover natural and historical sites. In Kyushu, they visit the Nabe Waterfall, formed by an ancient volcanic eruption, and the 400-year-old Takamori-dono cedars, which carry a tragic samurai legend. They also explore the &\#x27;Sky Torii&\#x27; at Kura Take Shrine, offering panoramic views, and the &\#x27;Oriental Niagara&\#x27; of Hara Waterfall, set in farmland. Nearby, they find centuries-old cliff Buddhas with vivid colors. The journey continues to the sunset at Magi Beach, where tidal flats mirror the sky, and the abandoned octagonal tunnel of a defunct railway. On Amami Oshima, they encounter the heart-shaped rock pool \(though obscured by sand\), the clear waters of Ohama Beach, and the dramatic cape of Miyaguzaki. They hike through the primeval forest of Kinzoku, spotting the endemic Otton frog, and paddle through the second-largest mangrove forest in Japan. At night, they search for the rare Amami rabbit, also encountering the Amami Ishikawa frog and a habu snake. Despite foggy weather at Honohoshi Coast, they discover remnants of a shrimp farm. The journey ends with a panoramic view from Kochiyama Observatory and a quiet sunset, capturing the island&\#x27;s serene beauty.

**「Takeaway」** The author concludes that both Kyushu&\#x27;s hidden gems and Amami Oshima&\#x27;s diverse landscapes offer profound experiences beyond typical tourist spots. The journey underscores the value of spontaneous exploration and the deep connection to nature and history found in these less-traveled places.

**Tags**: `#Japan travel`, `#Kyushu`, `#Amami Oshima`, `#travelogue`, `#sightseeing`

---

<a id="item-tech-blog-4"></a>
### [Community Digest: NuPhy Keyboard and Anti-Algorithm Info Sources](https://sspai.com/post/114327) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · Sep 8, 09:00

**「Background」** In this community roundup, the author highlights two user submissions: a hands-on review of a NuPhy magnetic switch keyboard obtained through a lucky box promotion, and a discussion on building &\#x27;anti-feed&\#x27; information sources to resist algorithmic content. The keyboard review offers personal impressions rather than deep technical analysis, while the discussion aggregates user opinions on avoiding algorithmic feeds.

**「Solution」** The keyboard review details the NuPhy BH65, a 65% all-aluminum magnetic switch keyboard with Gateron magnetic Jade Pro switches, 8000Hz polling, and 16000Hz scanning. The author notes its solid build and responsive feel in games like Valorant, but finds it heavy \(1.2kg\), wired-only, and less comfortable for typing due to higher actuation force. The &\#x27;anti-feed&\#x27; discussion presents two main strategies: self-hosted RSS \(Miniflux, FreshRSS\) with agent-based filtering, and psychological tricks like disabling personalized recommendations or using ad-supported versions to reduce engagement. Users also emphasize following credible sources, avoiding social media algorithms, and curating content manually.

**「Takeaway」** The author concludes that while the NuPhy keyboard offers good value at the discounted lucky box price, it is not worth the original price for non-gamers. For information consumption, the community suggests that proactive curation and deliberate &\#x27;disgust feedback&\#x27; can effectively counter algorithmic feeds, though these are personal preferences rather than universal solutions.

**Tags**: `#community digest`, `#keyboard review`, `#information sources`, `#RSS`, `#product impressions`

---