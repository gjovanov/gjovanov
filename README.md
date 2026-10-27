# 👋 Hi, I'm Goran

🚀 Building **[Roomler](https://roomler.ai)** — open-source remote desktop and a WireGuard mesh, in one daemon.

[![Discord](https://img.shields.io/badge/Discord-Join-5865F2?logo=discord&logoColor=white)](https://discord.gg/UBMX26MCq)
[![Docs](https://img.shields.io/badge/docs-roomler.ai%2Fdocs-009688)](https://roomler.ai/docs/)
[![Releases](https://img.shields.io/github/v/release/gjovanov/roomler-ai?filter=agent-*&label=agent)](https://github.com/gjovanov/roomler-ai/releases)

Roomler replaces **Tailscale + TeamViewer + Microsoft Teams** with one
open-source daemon and one web app: a private WireGuard mesh between your
machines, browser-based remote desktop with nothing to install on the viewing
side, and team chat + video on top — self-hosted free on unlimited devices, or
hosted at [roomler.ai](https://roomler.ai).

[![Roomler demo](https://raw.githubusercontent.com/gjovanov/roomler-ai/master/docs/assets/demo-preview.gif)](https://github.com/gjovanov/roomler-ai "A Windows 11 desktop, live in a browser tab, pinging a MacBook across the encrypted mesh")

---

## 🔧 What it replaces

| If you use… | …for | Roomler does it |
| --- | --- | --- |
| **TeamViewer / AnyDesk** | reaching a desktop | browser-based, consent-gated, works through corporate firewalls |
| **Tailscale / ZeroTier** | a private network between machines | WireGuard mesh, stable IPs, MagicDNS, exit nodes |
| **Slack + Zoom** | the team layer | rooms, chat, HD video calls — same server, same accounts |

Not a claim that it beats each of those at its own game — a claim that you stop
running three things, on one identity, with one agent. Full picture:
**[github.com/gjovanov/roomler-ai](https://github.com/gjovanov/roomler-ai)**

## 📖 Quick start

```bash
git clone https://github.com/gjovanov/roomler-ai.git && cd roomler-ai
cp .env.selfhost.example .env.selfhost      # fill in 4 values; 2 are `openssl rand -hex 32`
docker compose -f docker-compose.selfhost.yml --env-file .env.selfhost up -d
```

Free and unlimited, self-hosted — same code as the hosted service, no crippled
community build. Or skip the install and start a workspace at
[roomler.ai](https://roomler.ai), free for 3 devices.

## ⚖️ License

A split license, on purpose: the **server you'd host** is AGPL-3.0, and
everything you **install on a machine** (agent, CLI, desktop apps) is MPL-2.0 —
so MSPs and IT providers can build tooling around the agent without copyleft.
Details: [LICENSING.md](https://github.com/gjovanov/roomler-ai/blob/master/LICENSING.md).

## 📫 Get in touch

- 💬 **Discord:** **[discord.gg/UBMX26MCq](https://discord.gg/UBMX26MCq)**
- 🌐 **Roomler:** **[roomler.ai](https://roomler.ai)**
- 📦 **Source:** **[github.com/gjovanov/roomler-ai](https://github.com/gjovanov/roomler-ai)**

---

⭐ If Roomler is useful to you, consider starring the repo and joining the Discord!
