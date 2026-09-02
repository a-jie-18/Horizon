---
layout: default
title: "Horizon Summary: 2026-09-02 (EN)"
date: 2026-09-02
lang: en
---

> From 30 items, 3 important content pieces were selected

---

**Technology Blog**
1. [Extending Windows Update Pause via PowerShell](#item-tech-blog-1) ⭐️ 6.0/10
2. [Understanding Isn&\#x27;t Change: The Power of Reps](#item-tech-blog-2) ⭐️ 5.0/10
3. [A Decade of Daily Cannabis Use: One User&\#x27;s Struggle to Quit](#item-tech-blog-3) ⭐️ 5.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Extending Windows Update Pause via PowerShell](https://sspai.com/post/80562) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Sep 2, 07:22

**「Background」** Windows 10 and 11 push updates frequently, and the built-in pause feature only allows a maximum of 35 days. For users working on long projects, this can lead to unwanted restarts and potential data loss. The author, Levinson, experienced this firsthand and sought a way to extend the pause period beyond the standard limit.

**「Solution」** Levinson discovered that Windows Update stores its pause settings in the registry under HKLM:\\SOFTWARE\\Microsoft\\WindowsUpdate\\UX\\Settings. By using PowerShell to modify three registry values—PauseUpdatesExpiryTime, PauseFeatureUpdatesEndTime, and PauseQualityUpdatesEndTime—you can set a custom pause end date far beyond 35 days. The script converts a desired date \(e.g., 2030-01-01\) to UTC and formats it in ISO 8601 before writing it to these keys. The article provides step-by-step instructions: first pause updates via the Settings UI, then run the PowerShell command as administrator, and finally verify the new pause date in Settings. This method is flexible, allowing any future date, and works even though the UI&\#x27;s calendar picker has changed. The author notes that while this tweak is useful, it&\#x27;s important to remember to resume updates after the project is done to avoid missing critical security patches.

**「Takeaway」** The author&\#x27;s core point is that while Windows&\#x27; default pause limit is restrictive, a simple registry tweak via PowerShell offers a practical workaround for users who need longer control over update timing. This approach is especially valuable for professionals managing complex projects without dedicated IT support.

**Tags**: `#Windows Update`, `#PowerShell`, `#Registry`, `#System Administration`, `#Productivity`

---

<a id="item-tech-blog-2"></a>
### [Understanding Isn&\#x27;t Change: The Power of Reps](https://www.reddit.com/r/selfimprovement/comments/1w5eiy2/i_spent_two_years_knowing_exactly_what_was_wrong/) ⭐️ 5.0/10

reddit · r/selfimprovement · /u/Plus\_Ad3379 · Sep 2, 16:02

**「Background」** The author spent two years knowing exactly what was wrong with them—procrastination, dopamine loops, the knowing-doing gap—yet made no progress. They realized that understanding had become a comfortable substitute for action, keeping the urgency of change at bay.

**「Solution」** The author explains that the brain has two systems: one for knowing and planning, another for doing and executing. Reading and insight only feed the knowing side, while the doing side develops solely through reps—especially doing hard things when quitting feels reasonable. They found that no new framework helped; instead, they committed to one hard physical task weekly with no external goal or audience. Around week four or five, the resistance to starting lost its authority, not because the physical task mattered, but because it trained the nervous system to override comfort signals in low-stakes conditions. The knowing-doing gap persists, but they now close it with reps rather than more understanding.

**「Takeaway」** The author&\#x27;s core insight is that understanding one&\#x27;s problems can be the most sophisticated form of avoidance, and real change requires building the &\#x27;doing&\#x27; system through repeated action, not additional insight.

**Tags**: `#knowing-doing gap`, `#self-improvement`, `#behavior change`, `#personal insight`, `#action vs understanding`

---

<a id="item-tech-blog-3"></a>
### [A Decade of Daily Cannabis Use: One User&\#x27;s Struggle to Quit](https://www.reddit.com/r/selfimprovement/comments/1w5p7b8/chronically_high_for_almost_10_years_how_do_i_put/) ⭐️ 5.0/10

reddit · r/selfimprovement · /u/mia-bean · Sep 2, 22:22

**「Background」** The author, a high-functioning professional and graduate student, has been using cannabis daily for nearly a decade, starting at age 19. Despite external success, they struggle with executive function, motivation, and emotional regulation, and suspect their symptoms are tied to Cannabis Use Disorder rather than their ADHD or depression diagnoses.

**「Solution」** The author details their failed attempts to quit, including a six-month switch from vape pens to flower and edibles, which reduced use but did not eliminate cravings. They describe the unique pull of vape pens, which deliver a rapid, intense high that other forms cannot match, and note that even gabapentin prescribed for withdrawal did not curb the desire. They also discuss using alcohol to compensate, raising concerns about cross-addiction. The author acknowledges the role of trauma, family history of addiction, and co-occurring mental health conditions, and recognizes that quitting requires addressing the underlying needs the substance serves, but they have not yet found a sustainable replacement.

**「Takeaway」** The author&\#x27;s story illustrates that cannabis use disorder can persist despite high functioning, and that quitting is complicated by the substance&\#x27;s role in emotional regulation and the difficulty of replacing it with healthier habits. It underscores the need for comprehensive support that addresses both addiction and underlying mental health issues.

**Tags**: `#cannabis use disorder`, `#addiction`, `#mental health`, `#personal narrative`, `#self-improvement`

---