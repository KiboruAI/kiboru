# 🔴 KIBORU — AI Agent Army

> Your personal AI commander with a team of specialist agents. Powered by OpenClaw. Works with any AI model.

KIBORU is an open-source multi-agent AI system built on [OpenClaw](https://github.com/openclaw/openclaw). Instead of one general AI, KIBORU gives you a team — each agent specialized, all coordinated by KIBORU as the chief orchestrator.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Built on OpenClaw](https://img.shields.io/badge/Built%20on-OpenClaw-red)](https://github.com/openclaw/openclaw)
[![X](https://img.shields.io/badge/X-@KiboruAi-black)](https://x.com/KiboruAi)

---

## The Team

| Agent | Name | Specialty |
|---|---|---|
| 👑 KIBORU | Chief | Orchestrator — routes and coordinates all agents |
| 📅 Clio | Scheduler | Schedules, reminders, time management |
| 🔍 Nova | Researcher | Web research, analysis, fact-finding |
| ◎ Sol | On-chain | Solana wallets, token data, on-chain activity |
| ✉ Hermes | Comms | Email, Telegram, notifications |
| 🧠 Aria | Memory | Persistent memory, user profile, context |

---

## Choose Your AI Model

KIBORU works with **any AI provider** — use whatever you already have access to.

| Provider | Model | Notes |
|---|---|---|
| **Anthropic** | Claude Sonnet | Recommended — best for complex tasks |
| **OpenAI** | GPT-4o | Great alternative |
| **Groq** | Llama 3.3 70B | Fast & affordable |
| **Google** | Gemini 2.0 Flash | Good balance |
| **Ollama** | Llama 3.2, Qwen, etc. | Free, runs on your VPS |
| **OpenRouter** | 100+ models | One key, many models |

Just uncomment the provider you want in your `.env` file — that's it.

---

## Quick Start

### Prerequisites
- Docker + Docker Compose
- API key from any supported AI provider (or Ollama for free)
- Telegram Bot token (from [@BotFather](https://t.me/BotFather))

### 1. Clone the repo
```bash
git clone https://github.com/KiboruAI/kiboru.git
cd kiboru
```

### 2. Configure environment
```bash
cp .env.example .env
nano .env   # uncomment your preferred AI provider & add keys
```

### 3. Deploy
```bash
docker compose up -d
```

### 4. Connect Telegram
```bash
docker compose run --rm kiboru-gateway openclaw channels add \
  --channel telegram \
  --token YOUR_BOT_TOKEN
```

### 5. Open dashboard
Visit `http://your-vps-ip:3000` and paste your gateway token.

Your army is live. 🔴

---

## Architecture

```
User (Telegram / Web)
        │
        ▼
   KIBORU (Orchestrator)
        │
   ┌────┴────┬──────┬──────┬──────┐
   ▼         ▼      ▼      ▼      ▼
 Clio      Nova    Sol  Hermes  Aria
Scheduler Research Onchain Comms Memory
        │
        ▼
  Your AI Model
(Claude / GPT / Gemini / Ollama / Groq)
```

---

## Agent Packs (Coming Soon)

Agent packs are bundles of specialized agents for specific lifestyles. Unlock with $KIBORU token (coming soon).

- 🏃 **Healthy Life Pack** — workout scheduler, meal planner, habit tracker, sleep reminders
- 🎬 **Creator Pack** — shoot schedule, video concepts, caption writer, editing briefs
- ◎ **Crypto Pack** — token monitor, wallet tracker, alpha research, dev wallet watcher
- 📚 **Student Pack** — study schedule, research assistant, deadline tracker

---

## VPS Recommendations

| Provider | Plan | Price | Notes |
|---|---|---|---|
| **Hostinger** | KVM 2 | ~$7/mo | 1-click Docker, easiest setup |
| **Hetzner** | CX22 | ~€4/mo | Best value, 2 vCPU 4GB RAM |
| **DigitalOcean** | Basic | $6/mo | 1-click OpenClaw droplet |

Minimum: 1 vCPU, 2GB RAM. Recommended: 2 vCPU, 4GB RAM.

---

## Community

- Website: [kiboru.xyz](https://kiboru.xyz)
- X: [@KiboruAi](https://x.com/KiboruAi)
- GitHub: [KiboruAI/kiboru](https://github.com/KiboruAI/kiboru)

---

## Contributing

Contributions welcome! You can:
- Submit new agent SOUL.md templates
- Build and share agent packs
- Report issues or suggest features

See [CONTRIBUTING.md](docs/CONTRIBUTING.md) for guidelines.

---

## License

MIT — free to use, modify, and distribute.

---

*Built with ❤️ on OpenClaw · Any model. Your stack. Your army.*
