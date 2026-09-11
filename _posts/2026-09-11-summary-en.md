---
layout: default
title: "Horizon Summary: 2026-09-11 (EN)"
date: 2026-09-11
lang: en
---

> From 45 items, 1 important content pieces were selected

---

**Technology Blog**
1. [A Teacher&\#x27;s Timetable App Built on School Schedules](#item-tech-blog-1) ⭐️ 4.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [A Teacher&\#x27;s Timetable App Built on School Schedules](https://sspai.com/post/114384) ⭐️ 4.0/10

rss · 少数派 \(生活方式与效率\) · Sep 10, 06:51

**「Background」** After the timetable app iStudiez Pro shut down and other options failed to fit his needs, teacher and SwiftUI learner Tao\_Sway set out to build his own teacher-focused timetable app, &quot;下一节&quot; \(Next Class\). The article explains the design rationale behind it rather than its implementation.

**「Solution」** The author&\#x27;s central insight is that teachers schedule by school timetable, not by clock time: he records &quot;Wednesday period 3,&quot; not &quot;Wednesday 10:00.&quot; Because his own school used four different timetables during 2025-2026, a calendar would force him to adjust every class whenever the schedule changed. His app instead treats the timetable as the base axis, so switching timetables automatically shifts class times; teachers create a new timetable from an old template and set a switch date, and classes before that date keep the old times while later ones use the new table. The app also handles cancellations, moving a class to another period \(optionally permanently\), and odd/even-week arrangements, all within the timetable page. A &quot;Today&quot; page shows which class is next and how much free time remains before it, and allows brief notes on each class. The author reports that pre-launch features included Word-based timetable prefill, Excel timetable import, automatic statutory holiday adjustments, and whole-week scheduling on one page, but feedback from teachers on Xiaohongshu revealed more complex needs than he anticipated: different timetables on different days within one week, teaching two classes at once, three-week rotation cycles, and duty-type non-teaching arrangements, which the current version does not support well.

**「Takeaway」** The author argues that for teachers, the school timetable rather than clock time is the real scheduling axis, and that designing around it makes daily teaching life more manageable. He acknowledges the app still falls short of the full range of teacher needs and plans to keep updating it.

**Tags**: `#education-technology`, `#scheduling`, `#app-design`, `#product-rationale`, `#SwiftUI`

---