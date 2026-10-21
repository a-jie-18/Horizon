---
layout: default
title: "Horizon Summary: 2026-10-21 (EN)"
date: 2026-10-21
lang: en
---

> From 34 items, 5 important content pieces were selected

---

**Technology Blog**
1. [Firefox Nova&\#x27;s Aborted UI Modernization and Pixel VoLTE](#item-tech-blog-1) ⭐️ 6.0/10
2. [vivo Buds Clip Review: A Late but Solid Clip-Style Earbud](#item-tech-blog-2) ⭐️ 6.0/10
3. [BenQ MA270S and MA320U: A Mac Dual-Monitor Setup](#item-tech-blog-3) ⭐️ 4.0/10
4. [紫毫: A Rime-Based iOS Input Method With Typo Correction](#item-tech-blog-4) ⭐️ 4.0/10
5. [Urges as Forecasts: What a No-Dinner Retreat Revealed](#item-tech-blog-5) ⭐️ 4.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Firefox Nova&\#x27;s Aborted UI Modernization and Pixel VoLTE](https://sspai.com/prime/story/inside-release-notes-261020) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Oct 20, 10:01

**「Background」** Firefox has long oscillated between chasing design trends and preserving the simplicity and efficiency valued by its technical users. The Nova redesign, shipped with Firefox 157 in late September, was Mozilla&\#x27;s largest visual update since Proton in 2021, intended to modernize the browser and better accommodate vertical tabs, tab groups, and split view.

**「Solution」** Nova redraws icons, rounds toolbar controls, turns tabs into pills, and adds a smoky-purple gradient theme with a glow around the selected tab; the sidebar now reads as an extension of the toolbar rather than a separate panel. Early Nova builds were far more radical, splitting the browser into floating rounded regions with gaps between toolbar, sidebar, and content, echoing Arc-style layouts. After negative feedback, Mozilla abandoned that floating design—a reasonable retreat, the author argues, because decorative gaps yield only trendy screenshots while costing precision and screen space in a content-centric tool. The result is a somewhat inconsequential update, differing from Proton mainly in rounder buttons and pervasive purple. Still, Nova restores the compact density layout \(Settings &gt; Appearance &gt; Window density\), whose tab height is even a few pixels shorter than Proton&\#x27;s, and introduces Mozilla&\#x27;s Acorn design system, where spacing, color, type, and radius are standardized as JSON design tokens, replacing hard-coded CSS and syncing desktop and mobile updates with better dark-mode support. Users can temporarily revert via about:config \(browser.nova.enabled=false for Proton UI; sidebar.revamp for the old sidebar, incompatible with vertical tabs\), an option Mozilla says will remain through late 2027; installing the official Firefox Proton theme restores the older restrained palette.

**「Takeaway」** Nova is neither as bad as critics claim nor as advanced as Mozilla&\#x27;s modernization pitch suggests; its development reflects Firefox&\#x27;s enduring tension between appealing to mainstream users and retaining its geek community.

**Tags**: `#browser UI design`, `#Firefox`, `#design systems`, `#release notes`, `#mobile networking`

---

<a id="item-tech-blog-2"></a>
### [vivo Buds Clip Review: A Late but Solid Clip-Style Earbud](https://sspai.com/post/115475) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Oct 20, 09:30

**「Background」** vivo was the last major Chinese phone brand to release a clip-style open earbud, arriving after rivals like Sony and Nothing had already shipped such products. TDS Studio, reviewing a self-purchased unit, asks whether Buds Clip continues vivo&\#x27;s pattern of arriving late with higher polish, as its TWS 5 series had done.

**「Solution」** The author finds a conventional front/rear-module-plus-C-bridge design weighing 5.2g, with IP55 protection and a flatter rear module lacking the ear-contour curve some rivals add; long-term comfort \(about 2h\) was slightly better than LUNA, Xiaomi&\#x27;s clip and Enco Clip2, though fit angle proved unusually sensitive. Controls rely on panel touch plus whole-body tap recognition, and the author reports roughly one or two misreads in every five taps, plus mild lag. Call quality via dual mics plus a bone-conduction mic was stable and clear, with audible algorithm intervention under noise or side/back wind. On a BES2710IHC controller supporting SBC/AAC/LDAC/LC3, LDAC stayed largely stable to 8.5m through a load-bearing wall, with dropouts beyond 9m; AAC was stable to about 10m on both Xperia 1 V and iPhone 17. The claimed 70ms low-latency mode coexists with LDAC. Measured battery was 5h30m on LDAC versus just over 10h on AAC at 50% volume, matching vivo&\#x27;s AAC-based 10h/42h claim; charging held about 2.2W early then 0.8–1.1W. Sound was balanced and natural with slightly bright upper mids, good separation and soundstage layering for the category, and spatial audio that the author calls top-tier among clip earbuds; leak control was only average, consistent with its higher output. At the 500–600 yuan range, the author calls it one of the most worthwhile clip earbuds for digital buyers and recommends the wired-charging version over paying 100 yuan more for wireless.

**「Takeaway」** The author concludes that Buds Clip matches flagship clip earbuds in sound and avoids obvious weaknesses in signal and fit, with only control-recognition polish lagging, reinforcing vivo&\#x27;s broader pattern of well-rounded, reasonably priced earbuds across price tiers.

**Tags**: `#wireless earbuds`, `#product review`, `#audio hardware`, `#battery testing`, `#bluetooth codecs`

---

<a id="item-tech-blog-3"></a>
### [BenQ MA270S and MA320U: A Mac Dual-Monitor Setup](https://sspai.com/post/116661) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · Oct 20, 07:07

**「Background」** Laptop screens are too cramped for multi-track timelines, color panels, and previews, so external monitors remain essential for post-production work. Yet matching a third-party display to Apple&\#x27;s look is hard: identical sRGB, DCI-P3, and ΔE figures still yield visible differences in shadow detail, contrast, and color cast, and the broadcast-industry fix—controlled lighting, hoods, calibrators, reference monitors—is impractical for individual creators.

**「Solution」** The author treats Apple devices as a practical &quot;color ruler&quot; rather than an absolute standard, since Apple&\#x27;s ecosystem carries most digital content and its rendering favors natural-light perception with gentle shadow rolloff. BenQ&\#x27;s MA series targets this: M-book mode plus Display Pilot 2 auto-syncs ICC profiles per Mac model. The 32-inch 4K MA320U uses a matte panel that scatters reflections, while the 27-inch 5K MA270S uses a Nano Gloss low-reflection coating with 2000:1 native contrast, closer to the MacBook Pro&\#x27;s glass. The MA270S also adjusts brightness and color temperature to ambient light, which can be disabled for fixed-condition editing. The key technical point is scaling: at 2560×1440 HiDPI, a 4K panel must render a 5120×2880 image and resample it down, a non-integer ~1.5× mapping that slightly softens text and fine lines; a 5K panel maps each logical point to exactly 2×2 physical pixels with no final resample, giving crisper edges. In practice the author runs the MA270S center as the main display and the MA320U beside it, connected by a single Thunderbolt cable to the MacBook Pro—the MA270S passes through Thunderbolt 4 and delivers up to 96W reverse charging, with the MA320U daisy-chained from its rear port. Display Pilot 2 lets Mac F1/F2 and F11/F12 keys control brightness and volume, syncs brightness across both panels, and binds color mode, low blue light, and volume to macOS Focus modes via FocuSync. The author notes these are subjective impressions and vendor claims without independent measurement, and concludes a good 4K display still suffices for most work.

**「Takeaway」** The author&\#x27;s larger point is that 5K&\#x27;s real advantage for Mac users is integer 2× HiDPI rendering, not just pixel density, and that BenQ&\#x27;s MA series mainly reduces the friction of matching a third-party screen to Apple&\#x27;s look. Upgrading is worthwhile only if the current display already feels unsatisfying.

**Tags**: `#monitors`, `#macOS HiDPI scaling`, `#color management`, `#hardware review`, `#desk setup`

---

<a id="item-tech-blog-4"></a>
### [紫毫: A Rime-Based iOS Input Method With Typo Correction](https://sspai.com/post/116430) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · Oct 20, 02:34

**「Background」** Rime users on Mac and Windows who move to iPhone lose the experience of owning their dictionaries and tuning their own schemas, forced back to the system keyboard or ad-supported, network-connected third-party options. The author built 紫毫 \(Zihao\) to close that gap: a Rime-engine iOS input method with 雾凇拼音 built in, designed for iPhone, iPad, and iPhone Duo.

**「Solution」** On first launch the app deploys 雾凇拼音 locally and downloads a roughly 6.8 MB sentence-level language model tuned on Wikipedia Chinese colloquial text. It supports 26-key full pinyin, nine-key, and 小鹤双拼 \(with radical-based auxiliary filtering\), plus date, amount, and symbol shortcuts. Users can import Rime config folders, ZIPs, YAML, or text dictionaries, or point at a public GitHub repo such as iDvel/rime-ice with scheduled auto-updates; schemas compile on-device, and user dictionaries sync through an iCloud folder that can be shared with 鼠须管 via sync\_dir. The author&\#x27;s main technical claim is touch-aware correction layered on top of Rime: it uses finger position plus pinyin rules to recover intended input while keeping the original spelling in candidates, with a hard rule that a validly spelled input always ranks first so correct typing is never &quot;corrected&quot; away. In the author&\#x27;s own simulated tests, sentences with two mistyped letters rose from 36% to 56% first-try accuracy and three errors from 26% to 53%, with no correctly typed sentences broken. A separate ~5 MB on-device model reads preceding context to pick among homophones \(e.g., 输血 vs. 数学\). All typing, correction, learning, and both models run locally; AI features require the user&\#x27;s own API keys and, since 1.0.9, mask phone numbers, IDs, bank cards, emails, and verification codes with placeholders before sending.

**「Takeaway」** The author argues that a Rime-based iOS keyboard can preserve local dictionary ownership and schema control while adding touch-specific correction and context-aware candidate ranking, all without sending keystrokes off-device. The correction figures are self-reported simulations without published methodology, so they should be read as the developer&\#x27;s claim rather than independently verified results.

**Tags**: `#input-method`, `#rime`, `#ios`, `#typo-correction`, `#privacy`

---

<a id="item-tech-blog-5"></a>
### [Urges as Forecasts: What a No-Dinner Retreat Revealed](https://www.reddit.com/r/selfimprovement/comments/1xaut3j/urges_pass_if_you_wait_them_out_is_right_but/) ⭐️ 4.0/10

reddit · r/selfimprovement · /u/Deep\_Ad1959 · Oct 20, 15:14

**「Background」** Standard craving advice says to sit with an urge until it peaks and passes, and the author has seen this work for phones and snacks. But a repeated no-dinner schedule on meditation retreats suggested something underneath that advice: the urge may be less a need than a learned expectation tied to a time slot.

**「Solution」** On six 10-day meditation courses, the author ate lunch as the main meal, had fruit and tea at 5pm as a new student, and then nothing until breakfast. The first couple of evenings were rough: hunger arrived at the same point each evening, and the author spent the evening sit negotiating with it. Around day three, the hunger simply stopped arriving—not because resistance improved, but because the body&\#x27;s forecast updated once nothing came at that time for a few days. The author extends this to phone and snack urges: waiting each one out also teaches the body that the slot is empty, and the first few nights are the expensive ones because the old schedule is still running. The author notes being neither a teacher nor a nutrition person, just someone who has been hungry in a meditation hall more than once.

**「Takeaway」** The author&\#x27;s larger point is that urge-surfing may work not only by building willpower but by retraining the body&\#x27;s expectation schedule, so the craving eventually stops showing up at all.

**Tags**: `#cravings`, `#habit-formation`, `#self-improvement`, `#anecdotal-evidence`, `#behavior-change`

---