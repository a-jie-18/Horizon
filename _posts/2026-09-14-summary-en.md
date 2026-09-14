---
layout: default
title: "Horizon Summary: 2026-09-14 (EN)"
date: 2026-09-14
lang: en
---

> From 28 items, 1 important content pieces were selected

---

**Technology Blog**
1. [Building a HomeLab: A Personal Hardware Inventory](#item-tech-blog-1) ⭐️ 6.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Building a HomeLab: A Personal Hardware Inventory](https://sspai.com/post/113880) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Sep 13, 07:51

**「Background」** A software developer who started with a first NAS in 2019 documents the hardware behind his HomeLab — a home version of a cloud server running self-hosted services — motivated by keeping data and family photos off third-party cloud storage after a lapsed OSS subscription made his blog images unreachable. The article is the first in a series and covers only hardware, costs, and pitfalls; network, services, and backup details are deferred to later installments.

**「Solution」** The author&\#x27;s guiding principles are KISS, &quot;good enough,&quot; and avoiding an All-in-One \(&quot;All in Boom&quot;\) box: compute, storage, and network stay on separate machines so one failure doesn&\#x27;t take everything down, with dual telecom/Unicom gigabit lines as mutual redundancy. Important data goes on Synology NAS units — a DS218+ syncing files via Drive and a DS923+ backing it up, running media services and Docker, with a LaCie d2 for cold backup and a UPS — while less critical services run in Docker on second-hand gear. The main server is a ThinkStation M920x Tiny \(i7-8700, 64G RAM, dual 10G optical NIC\) running Ubuntu Server with Docker and KVM/QEMU, hosting 40+ services and four VMs; a dual-E5 desktop with 256G RAM, a used 2080Ti and a Tesla P40 serves as the model-training rig but draws too much power to run 24/7. Network gear is mostly second-hand: Xiaomi routers for dual-WAN dial-up, several R2S/R5S/H28K OpenWrt boxes as bypass routers and WireGuard nodes, and a mix of 2.5G and 10G switches, with a 99-yuan/year Alibaba Cloud instance for a fixed public IP. The author is candid about tradeoffs: link aggregation doesn&\#x27;t actually work without a managed switch, the P40 is slow and sometimes unsupported by models, the 6500Pro has poor thermals, and the desktop mostly sits idle. Open questions include whether to go all-optical or all-copper for a future 10G switch, unfinished R5S fan control, and whether K8S is ever needed.

**「Takeaway」** The author&\#x27;s core thesis is that a HomeLab is best built as several independent machines rather than one do-everything box, accepting extra design and cost to protect data continuity — a tradeoff he considers worthwhile only for those who genuinely depend on their home services, since a casual setup needn&\#x27;t be this complex.

**Tags**: `#homelab`, `#nas`, `#networking`, `#self-hosting`, `#hardware`

---