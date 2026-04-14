# 🔴 KIBORU — AI Agent Army

> Your personal AI commander with a team of 5 specialist agents. Free to try. Open source to self-host.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Built on OpenClaw](https://img.shields.io/badge/Built%20on-OpenClaw-red)](https://github.com/openclaw/openclaw)
[![Telegram Bot](https://img.shields.io/badge/Telegram-@KiboruAI__bot-blue)](https://t.me/KiboruAI_bot)
[![Telegram Channel](https://img.shields.io/badge/Channel-@kiboruai-blue)](https://t.me/kiboruai)
[![X](https://img.shields.io/badge/X-@KiboruAi-black)](https://x.com/KiboruAi)

---

## Try it free

**Chat with KIBORU on Telegram → [t.me/KiboruAI_bot](https://t.me/KiboruAI_bot)**
No signup. No setup. Just chat.

Join the community → [t.me/kiboruai](https://t.me/kiboruai)

---

## The Team

| Agent | Name | Specialty |
|---|---|---|
| 👑 KIBORU | Chief | Orchestrator — routes and coordinates all agents |
| 📅 Kaze | Scheduler | Schedules, reminders, time management |
| 🔍 Riku | Researcher | Web research, analysis, fact-finding |
| ◎ Ren | On-chain | Solana wallets, token data, on-chain activity |
| ✉ Haru | Comms | Email, Telegram, notifications |
| 🧠 Miko | Memory | Persistent memory, user profile, context |

---

## Choose Your AI Model

KIBORU works with **any AI provider** — use whatever you already have.

| Provider | Model | Notes |
|---|---|---|
| **Anthropic** | Claude Haiku / Sonnet | Recommended |
| **OpenAI** | GPT-4o | Great alternative |
| **Groq** | Llama 3.3 70B | Fast & affordable |
| **Google** | Gemini 2.0 Flash | Good balance |
| **Ollama** | Llama 3.2, Qwen, etc. | Free, runs on your VPS |
| **OpenRouter** | 100+ models | One key, many models |

---

## Self-Host in 5 Minutes

### Prerequisites
- Docker + Docker Compose
- API key from any supported AI provider
- Telegram Bot token (from [@BotFather](https://t.me/BotFather))

### Deploy
```bash
git clone https://github.com/KiboruAI/kiboru.git
cd kiboru
cp .env.example .env
nano .env   # add your API key
docker compose up -d
```

### Connect Telegram
```bash
docker compose run --rm kiboru-gateway openclaw channels add \
  --channel telegram \
  --token YOUR_BOT_TOKEN
```

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
 Kaze      Riku    Ren   Haru   Miko
Scheduler Research Onchain Comms Memory
        │
        ▼
  Your AI Model
(Claude / GPT / Gemini / Ollama / Groq)
```

---

## Agent Packs (Coming Soon)

- 🏃 **Healthy Life Pack** — workout scheduler, meal planner, habit tracker
- 🎬 **Creator Pack** — shoot schedule, video concepts, caption writer
- ◎ **Crypto Pack** — token monitor, wallet tracker, alpha research
- 📚 **Student Pack** — study schedule, research assistant, deadline tracker

Packs will be unlockable via **$KIBORU token** (coming soon).

---

## Community

- Website: [kiboru.xyz](https://kiboru.xyz)
- Telegram Bot: [@KiboruAI_bot](https://t.me/KiboruAI_bot)
- Telegram Channel: [@kiboruai](https://t.me/kiboruai)
- X: [@KiboruAi](https://x.com/KiboruAi)
- GitHub: [KiboruAI/kiboru](https://github.com/KiboruAI/kiboru)

---

## Contributing

- Submit new agent SOUL.md templates
- Build and share agent packs
- Report issues or suggest features

See [CONTRIBUTING.md](docs/CONTRIBUTING.md) for guidelines.

---

## License

MIT — free to use, modify, and distribute.

---

*Any model. Your stack. Your army. 🔴*
