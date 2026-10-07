---
layout: default
title: "Horizon Summary: 2026-10-07 (EN)"
date: 2026-10-07
lang: en
---

> From 28 items, 1 important content pieces were selected

---

**Technology Blog**
1. [Self-Hosting Vaultwarden with Cloudflare Tunnel and Keyguard](#item-tech-blog-1) ⭐️ 6.0/10

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Self-Hosting Vaultwarden with Cloudflare Tunnel and Keyguard](https://sspai.com/post/115416) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · Oct 6, 10:00

**「Background」** After subscription price hikes pushed the author off Enpass, and with 1Password, LastPass, and KeePass each carrying their own drawbacks, the author turned to Bitwarden — but balked at paying extra for TOTP support and found the official clients unremarkable. Since a NAS already runs 24/7 at home, self-hosting Vaultwarden became the natural next step.

**「Solution」** Vaultwarden is a community-maintained, unofficial Bitwarden backend that is far lighter than the official .NET stack — typically under 100 MB of resident memory — while unlocking TOTP management and multi-user sharing directly from the server. The author deploys it via Docker on the NAS, mapping the container&\#x27;s /data directory to a real NAS folder for persistence and backup, changing ROCKET\_PORT or bridging port 80 to avoid conflicts, and setting DOMAIN to the public hostname. Because browsers enforce a secure-context policy, the Web Crypto API that the web vault depends on only works over HTTPS, so plain LAN IP access is rejected; rather than a reverse proxy, which is painful behind carrier-grade NAT, the author uses Cloudflare Tunnel to expose the service, obtaining SSL/TLS, DDoS protection, and access control for free. A cheap domain hosted on Cloudflare is recommended over the temporary trycloudflare.com addresses, which change on every restart. After registering, the author sets SIGNUPS\_ALLOWED to false to prevent strangers from creating accounts, and either sets a strong ADMIN\_TOKEN or deletes it entirely to close the /admin panel, since the vault rarely needs reconfiguration. Migration is done through the Tools &gt; Import page, with Enpass JSON importing cleanly; the author advises running the old manager in parallel before deleting anything. For mobile, the author switched to Keyguard, an open-source Bitwarden/KeePass-compatible client with better UI and passkey import, which can also take over Android 14&\#x27;s third-party autofill and keeps a local vault usable even when Cloudflare connectivity drops. The author notes Keyguard can bypass Bitwarden&\#x27;s frontend-only TOTP restriction for free users, though browser use may require manually copying codes.

**「Takeaway」** The author argues that self-hosting Vaultwarden with Cloudflare Tunnel and Keyguard yields a more controllable, freer password setup than commercial products, and that once the chain works, extending the same pattern to other services is straightforward.

**Tags**: `#self-hosting`, `#password-management`, `#Vaultwarden`, `#Cloudflare Tunnel`, `#Docker`

---