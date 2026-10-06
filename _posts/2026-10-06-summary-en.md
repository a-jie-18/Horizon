---
layout: default
title: "Horizon Summary: 2026-10-06 (EN)"
date: 2026-10-06
lang: en
---

> From 23 items, 1 important content pieces were selected

---

**Technology Blog**
1. [iOS 27 Notification Automation: Ten Practical Shortcuts Recipes](#item-tech-blog-1) ⭐️ 7.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [iOS 27 Notification Automation: Ten Practical Shortcuts Recipes](https://sspai.com/post/114536) ⭐️ 7.0/10

rss · 少数派 \(生活方式与效率\) · Oct 5, 02:59

**「Background」** iOS 27 adds notification automation to Shortcuts, letting any app that can post a notification act as a trigger — not just Calendar, Reminders, Mail, or Messages. Since notifications carry structured fields, the author argues this is less a new trigger than a whole new input layer for Shortcuts.

**「Solution」** Automations filter on three fields — title, subtitle, and body — and all conditions must match simultaneously. Because Shortcuts&\#x27; own &quot;Show Notification&quot; action maps fields differently than real notifications, the author advises reading the actual on-screen notification layout to identify which line is which; WeChat, for example, shows the contact name as title and the message as body. The output variable exposes app name, title, subtitle, body, and date for further branching. A prerequisite: the app&\#x27;s notifications must be enabled with Lock Screen or Notification Center display — banner-only won&\#x27;t run. The ten recipes include escalating reminders for a contact who messages repeatedly over 30 minutes \(approximating &quot;read&quot; via an Open App automation, since true read detection isn&\#x27;t possible\), wallpaper-overlaid badges to restore counts lost after custom app icons \(workable only on a single home screen; the alternative generated-icon method can&\#x27;t be easily deleted\), color-coded wallpapers rendered via HTML-to-image, per-contact ringtones, auto-translation of English notifications, an AI notification-summary database, payment-notification bookkeeping, scheduled WeChat sending via Reminders \(five-minute granularity unless created through Siri\), cross-brand smart-home bridging, and consolidating assigned Reminders onto the wallpaper. The author flags a key limitation: automation captures only displayed text, so truncated or ellipsized notifications — common in WeChat — yield incomplete content.

**「Takeaway」** The author&\#x27;s thesis is that notification automation shifts notifications from something a person reads and acts on into a structured input that Shortcuts can read, judge, and act upon — with the human judgment moved into the system where possible. The recipes are anecdotal and platform-specific, but the underlying pattern is broadly transferable.

**Tags**: `#iOS Shortcuts`, `#notification automation`, `#Apple ecosystem`, `#workflow automation`, `#practical tutorial`

---