<div align="center">

<img src="https://raw.githubusercontent.com/sassisouid/chativa/main/assets/chativa-logo.png" alt="Chativa Logo" width="120" />

# Chativa

### Self-Hosted, End-to-End Encrypted Team Messaging — with AI

**The privacy-first alternative to Slack and Microsoft Teams.**  
Your messages. Your server. Your rules.

[![Version](https://img.shields.io/badge/version-1.0.0-gold?style=flat-square)](https://github.com/sassisouid/chativa/releases/tag/v1.0.0)
[![License](https://img.shields.io/badge/license-Commercial-blue?style=flat-square)](LICENSE.txt)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-lightgrey?style=flat-square)](https://github.com/sassisouid/chativa/releases)
[![Download](https://img.shields.io/badge/download-Gumroad-orange?style=flat-square)](https://neuralsales.gumroad.com/l/chativa)

[⬇️ Download v1.0.0](https://github.com/sassisouid/chativa/releases/tag/v1.0.0) · [📖 Documentation](#installation) · [💬 Support](mailto:support@chativa.pro) · [🛒 Get Pro](https://neuralsales.gumroad.com/l/chativa)

</div>

---

## Why Chativa?

Most team messaging tools — Slack, Teams, Discord — store your conversations on **their** servers. You have no control over who reads your data, how long it's kept, or what happens if they get breached.

**Chativa is different.** It runs entirely on your own infrastructure. Every message is end-to-end encrypted before it leaves the sender's device. No third party can read your conversations — not even us.

> 💡 **Perfect for:** SMEs, legal firms, healthcare teams, agencies, and any business that handles sensitive information.

---

## See It in Action

<div align="center">

https://github.com/sassisouid/chativa/assets/chativa-demo.mp4

</div>

---

## Features

### 🔐 Privacy & Security
- **End-to-End Encryption (E2EE)** — RSA-2048 + AES-256-GCM on every message and file
- **Self-hosted** — Deploy on your own Windows machine or VPS. Zero data leaves your infrastructure
- **JWT Authentication** — 7-day tokens with server-side invalidation on logout
- **Rate limiting** — Built-in brute-force protection on all API endpoints

### 💬 Real-Time Messaging
- **1:1 and group chat** — Unlimited conversations with read receipts (✓ sent, ✓✓ read)
- **Voice messages** — Record and send audio clips up to 60 seconds
- **File sharing** — Send images, documents, audio, and video (up to 100 MB)
- **Message deletion** — Remove messages from both sides
- **@mentions** — Notify specific team members in group rooms

### 📞 Audio & Video Calls
- **WebRTC-powered** — Peer-to-peer calls with no relay server required
- **1:1 and group calls** — Up to 6 participants per call
- **Screen sharing** — Share your screen during any call
- **Full call controls** — Mute, camera toggle, hang up

### 🤖 AI-Powered Features (Gemini)
- **Conversation summaries** — Get a 3-point summary of any conversation instantly
- **Reply suggestions** — AI-generated response options based on context
- **AI chat widget** — Auto-reply to website visitors, escalate to human agents when needed
- **Per-project AI config** — Custom system prompts and personalities per widget

### 🧩 Embeddable Chat Widget
- **One-line integration** — Add live chat to any website with a single `<script>` tag
- **Lead capture** — Collect visitor name and email before starting a chat
- **Custom branding** — Match your brand colors and welcome message
- **AI auto-reply** — Handle visitor questions 24/7 without an agent

### ⚙️ Administration
- **Multi-language** — English, Français, Español
- **Role-based access** — Admin and Agent roles with granular permissions
- **System settings** — File limits, call quotas, AI configuration — all from the dashboard
- **Automatic updates** — One-click update notifications built in

---

## Free vs Pro

| Feature | Free | Pro |
|---------|:----:|:---:|
| Agents | Up to 3 | ✅ Unlimited |
| Projects / Widgets | 1 | ✅ Unlimited |
| Audio/Video Calls | 10 / month | ✅ Unlimited |
| AI Requests | 20 / day | ✅ 1,000 / day |
| Message History | 30 days | ✅ Unlimited |
| 1:1 & Group Chat | ✅ | ✅ |
| File Sharing | ✅ 10 MB | ✅ Configurable |
| E2EE Encryption | ✅ | ✅ |
| Widget Integration | ✅ | ✅ |
| AI Widget (Auto-reply) | ✅ | ✅ |
| Automatic Updates | ✅ | ✅ |
| Priority Support | ❌ | ✅ |
| Advanced Analytics | ❌ | ✅ |

👉 **[Get Pro on Gumroad](https://neuralsales.gumroad.com/l/chativa)**

---

## Installation

### Requirements

| Component | Minimum |
|-----------|---------|
| OS | Windows 10 / 11 (x64) |
| RAM | 4 GB |
| Disk | 500 MB free |
| Database | MongoDB 4.4+ (Atlas or self-hosted) |

### Quick Start (3 steps)

**1. Download and extract**
```
Chativa-E2EE-x64-v1.0.0.zip → Extract → Chativa.exe
```

**2. Run the setup wizard**

Double-click `Chativa.exe`. The 5-step wizard will guide you through:
- MongoDB connection (paste your Atlas URI or local connection string)
- Admin account creation
- First project setup
- (Optional) Pro license activation

**3. Open the dashboard**

The app opens automatically at `http://localhost:5000`. Invite your team via **Users → Add User**.

> 📖 For detailed instructions, see the [User Guide](https://github.com/sassisouid/chativa/releases/download/v1.0.0/Chativa-E2EE-x64-v1.0.0.zip) included in the release ZIP.

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Desktop shell | Electron 31 |
| Backend | Node.js + Express |
| Real-time | Socket.io |
| Database | MongoDB + Mongoose |
| Calls | WebRTC (peer-to-peer) |
| Encryption | RSA-2048 + AES-256-GCM |
| AI | Google Gemini API |
| Auth | JWT (jsonwebtoken) |

---

## Roadmap

- [x] v1.0.0 — Production stable release
- [ ] v1.1.0 — Admin UI for Cloudinary & Stripe configuration
- [ ] v1.1.0 — Advanced analytics dashboard
- [ ] v1.2.0 — macOS & Linux support
- [ ] v1.2.0 — Mobile companion app (iOS / Android)
- [ ] v2.0.0 — Multi-tenant SaaS mode

---

## Support

| Channel | Details |
|---------|---------|
| 📧 Email | [support@chativa.pro](mailto:support@chativa.pro) |
| 🐛 Bug Reports | [Issues](https://github.com/sassisouid/chativa/issues) |
| 💡 Feature Requests | [Discussions](https://github.com/sassisouid/chativa/discussions) |
| 📖 In-app Help | **Help → Documentation** inside the app |

When reporting a bug, please include your Windows version and the contents of `%APPDATA%\Chativa\chativa-debug.log`.

---

## License

Chativa is distributed under a **Commercial License**.  
Free Edition available with usage limits. Pro Edition requires a license purchased on [Gumroad](https://neuralsales.gumroad.com/l/chativa).

See [LICENSE.txt](LICENSE.txt) for full terms.

---

<div align="center">

**[⬇️ Download Free](https://github.com/sassisouid/chativa/releases/tag/v1.0.0)** · **[🛒 Upgrade to Pro](https://neuralsales.gumroad.com/l/chativa)** · **[📧 Contact](mailto:support@chativa.pro)**

*Built for teams that take privacy seriously.*

</div>
