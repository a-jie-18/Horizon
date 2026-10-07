---
layout: default
title: "Horizon Summary: 2026-10-07 (ZH)"
date: 2026-10-07
lang: zh
---

> 从 28 条内容中筛选出 1 条重要资讯。

---

**科技博客**
1. [自托管 Vaultwarden 与 Keyguard 密码管理实践](#item-tech-blog-1) ⭐️ 6.0/10

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [自托管 Vaultwarden 与 Keyguard 密码管理实践](https://sspai.com/post/115416) ⭐️ 6.0/10

rss · 少数派 \(生活方式与效率\) · 10月6日 10:00

**「背景」** 作者在 Enpass 订阅涨价后，需要为手中三四百条密码寻找新家：1Password 订阅昂贵、LastPass 安全记录堪忧、KeePass 跨平台体验碎片，而 Bitwarden 的 TOTP 等高级功能需付费。恰好家中有一台 24 小时开机的 NAS，于是作者转向自托管方案。

**「方案」** 作者选择社区维护的开源 Bitwarden 后端 Vaultwarden，因其镜像轻巧、常驻内存通常不过百兆，且能从后端解锁 TOTP 与多人共享等高级功能。部署上以 Docker 为主：将容器 /data 映射到 NAS 实体目录以持久化密码库，修改 ROCKET\_PORT 或把 80 端口映射到宿主机其他端口以避免冲突，并配置 DOMAIN 环境变量。由于浏览器安全上下文策略要求可信网络，非 localhost 访问必须走 HTTPS；面对国内家庭宽带多为大内网、反向代理门槛高的问题，作者推荐用 Cloudflare Tunnel 将内网服务映射出去，顺带获得证书、DDoS 防护与访问控制，并建议购买便宜域名托管到 Cloudflare，避免临时 trycloudflare 域名重启即变。安全加固方面，注册账号后应立即将 SIGNUPS\_ALLOWED 设为 false，防止陌生人注册甚至把服务当免费网盘；/admin 后台默认关闭，作者建议配置完成后直接删除 ADMIN\_TOKEN 彻底关闭。迁移时通过「工具-导入」选择 Enpass \(JSON\) 即可解析，并建议新旧工具并行一段时间再卸载。移动端作者改用第三方开源客户端 Keyguard，认为其 UI 与交互优于官方 App，可接管 Android 14 的第三方自动填充，并凭借本地密码库缓存在 Cloudflare 波动时仍可使用；作者还称 Bitwarden 并未在服务端封禁免费用户的 TOTP，只是前端未开放入口，Keyguard 可绕过该限制。

**「启示」** 作者认为，自托管服务虽听起来复杂，但跑通一次后其他服务万变不离其宗，能带来比商业成品更可控、更自由的使用体验；这套 Vaultwarden + Cloudflare Tunnel + Keyguard 的组合已稳定运行，可作为希望掌控数据的用户的参考。

**标签**: `#self-hosting`, `#password-management`, `#Vaultwarden`, `#Cloudflare Tunnel`, `#Docker`

---