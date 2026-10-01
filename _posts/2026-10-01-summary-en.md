---
layout: default
title: "Horizon Summary: 2026-10-01 (EN)"
date: 2026-10-01
lang: en
---

> From 38 items, 3 important content pieces were selected

---

**Technology Blog**
1. [Destiny 2 and Bungie&\#x27;s &quot;Train Station Theory&quot;](#item-tech-blog-1) ⭐️ 6.0/10
2. [2Do Rebuilt: A Modern Take on a Classic Task Manager](#item-tech-blog-2) ⭐️ 6.0/10
3. [Using AI Agents to Plan a Seven-Day Henan Road Trip](#item-tech-blog-3) ⭐️ 6.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Destiny 2 and Bungie&\#x27;s &quot;Train Station Theory&quot;](https://sspai.com/post/115070) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Sep 30, 14:32

**「Background」** Destiny 2 is a live-service shooter that shipped paid expansions roughly yearly, with smaller seasonal content in between. Writing as a player of over two thousand hours rather than a developer, the author asks how Bungie—the studio behind Halo—ended up neither closing the game gracefully nor reviving it, and traces that outcome to a production philosophy adopted years earlier.

**「Solution」** The author builds his account around &quot;train station theory,&quot; a term he attributes to Destiny 2 product manager Justin Truman&\#x27;s 2022 GDC talk. After a 2018 player-count decline following Curse of Osiris, Bungie shifted from shipping boxed products to running a service, and the 2018 expansion Forsaken showed the payoff: frequent small updates filling gaps between major releases, which the author says became the foundation of Destiny 2&\#x27;s activity model. The theory&\#x27;s core, as he describes it, is that a well-built train leaving late disrupts the whole station, so on-time departure matters more than the quality of any single car—Bungie would rather ship boring or broken content than delay. The author credits this with commercial success through The Final Shape, but argues it became a paradox: the expansions players remember best—Forsaken, The Witch Queen, The Final Shape—were all delayed, while the seasons that followed them repeated the same recycled activities. He cites Bloomberg&\#x27;s October 2023 report that The Final Shape slipped from February to June 2024, leaving the previous season running seven months, plus layoffs and the troubled Marathon. In May 2026 Bungie announced Destiny 2&\#x27;s final update on June 10 and, on June 25, layoffs and restructuring under Sony pressure. The author also points to an information gap: Forbes reporter Paul Tassi said almost the whole studio learned of the shutdown only when it was announced, and some staff were still building year-nine content. He notes the irony that the game&\#x27;s population briefly rose toward 25,000 after the announcement, while Marathon&\#x27;s peak had fallen to around 2,700.

**「Takeaway」** The author&\#x27;s conclusion is that live-service production rewards stable, predictable output, while creativity requires unpredictable iteration—and Bungie let the measurable goal of shipping on time crowd out the harder question of whether the content was worth playing. He frames Destiny 2&\#x27;s decline less as one leader&\#x27;s mistake than as a once-successful production method hardening into conflict with what the game actually needed, which the organization failed to correct.

**Tags**: `#live-service games`, `#game development`, `#Destiny 2`, `#Bungie`, `#post-mortem`

---

<a id="item-tech-blog-2"></a>
### [2Do Rebuilt: A Modern Take on a Classic Task Manager](https://sspai.com/post/115166) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Sep 30, 07:00

**「Background」** 2Do, a macOS-native task manager over a decade old, had grown functionally rich but visually dated, with dense controls and cramped spacing. After the developer announced a full Swift rewrite in 2021 and then went largely silent for years, many users assumed the promised new version would never arrive. It finally shipped in August.

**「Solution」** In this experience-based review, the author argues the rebuild keeps 2Do&\#x27;s defining flexibility while modernizing everything around it. The interface moves to a three-column layout with more whitespace, independent light/dark themes, adjustable density, and a Busy Days heatmap that shows calendar load when scheduling. Native multi-window support \(Control-Option-Command-N\) enables cross-window drag-and-drop of tasks, including onto the calendar bar or toolbar buttons, and mobile keeps its signature swipe-based three-pane navigation plus pinch-to-adjust density. Natural-language capture parses relative dates, durations like \[2h\], priorities, lists, tags, and locations, with quotes to escape keywords; the author notes Chinese alert parsing appears broken. Email capture was rewritten to a cloud forwarding address per client, and filtering now supports cross-dimension OR with parentheses, scoped list/tag groups, and search inheritance toggles. Notes gained Markdown, @\{task\} bidirectional links, and an extracted-links panel. The sync engine was fully rewritten: native iCloud sync \(no app-specific password\) now carries smart lists, tag groups, and attachments, with Apple Reminders and Todoist two-way sync for other platforms, though third-party sync loses advanced metadata by writing some properties as plain text into notes. Pricing is a hybrid: $9.99 iOS, $19.99 iPadOS, and $49.99 macOS with 18 months of feature updates, after which the app keeps working and bug fixes continue, with optional $39.99/18-month renewals.

**「Takeaway」** The author&\#x27;s conclusion is that 2Do remains unmatched among Mac task managers for the freedom of its metadata and filtering, and that the rewrite finally makes that power usable on modern systems. The buyout-plus-maintenance pricing is framed as a healthier, more sustainable model for both users and an independent developer than pure subscription.

**Tags**: `#task-management`, `#GTD`, `#macOS`, `#software-review`, `#sync`

---

<a id="item-tech-blog-3"></a>
### [Using AI Agents to Plan a Seven-Day Henan Road Trip](https://sspai.com/post/114945) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Sep 30, 03:02

**「Background」** Planning a holiday trip is high-density information work: filtering the few details that actually drive decisions out of a flood of notes, guides, and official policies. One-shot prompts like &quot;plan me a Z-day trip to Y&quot; produce plausible itineraries that ignore human stamina, miscalculate holiday traffic and queue times, and stay vague on hotels and food. The author, a self-described planner who travels with two elderly parents, one driver, and an EV, wanted a workflow that kept judgment human while delegating the legwork.

**「Solution」** The author&\#x27;s method inverts the usual order: sketch the main line yourself, then have an agent refine it. Four principles guide the filtering—separate signal \(information that changes a concrete decision\) from noise; prefer first-hand sources such as official ticket pages over second-hand influencer notes; trust real commenters over algorithm-boosted posts; and remember that input quality determines output quality. The pipeline runs one way: pick a theme, choose cities, select attractions, derive the route and ticket deadlines, then work backward to hotels and food along the driving line. Xiaohongshu&\#x27;s AI assistant Diandian drafts candidates from real community notes with traceable sources; a local agent \(ZCode, Claude Code, Workbuddy\) then merges the material, reads screenshots of price boards and route maps, and iterates. Amap&\#x27;s map mini-program visualizes spatial relationships so out-of-the-way stops can be cut. Output is a single HTML file with an overview page and per-day tabs, small enough to send via WeChat and open offline. The Henan trip—Luoyang, Dengfeng, Kaifeng—shows the payoff: the agent caught a ticket-rule conflict at Qingming Shanghe Park \(National Day single-entry rules versus the usual three-day re-entry, resolved by buying the evening show ticket first\), and the author rerouted a night drive to Dengfeng to match her night-owl driver&\#x27;s rhythm. The author is candid about limits: agents hallucinate geography \(one placed a Kaifeng restaurant in Luoyang\), rely on stale policy data, and tend to agree rather than challenge, so a deliberate adversarial review—asking the agent to critique the plan as a professional guide—is essential. Hotel bookings favor early-bird, same-day-cancellable rates; food lists are screened for pre-made dishes and marketing posts, with one or two fixed meals per day and the rest left flexible.

**「Takeaway」** The author&\#x27;s thesis is that agents should absorb the labor of searching, calculating, and formatting, while the traveler keeps every decision about where to go, with whom, and why. The value of the workflow lies less in any single tool than in that division of labor and the discipline of returning to primary sources.

**Tags**: `#AI agents`, `#travel planning`, `#prompt engineering`, `#workflow design`, `#information filtering`

---