# 🔴 KIBORU — AI Agent Army

> Your personal AI commander with a team of specialist agents. Powered by OpenClaw.

KIBORU is an open-source multi-agent AI system built on [OpenClaw](https://github.com/openclaw/openclaw). Instead of one general AI, KIBORU gives you a team — each agent specialized, all coordinated by KIBORU as the chief orchestrator.

---

## The Team

| Agent | Name | Specialty |
|---|---|---|
| 👑 KIBORU | Chief | Orchestrator — routes and coordinates all agents |
| 📅 Scheduler | Clio | Schedules, reminders, time management |
| 🔍 Researcher | Nova | Web research, analysis, fact-finding |
| ◎ On-chain | Sol | Solana wallets, token data, on-chain activity |
| ✉ Comms | Hermes | Email, Telegram, notifications |
| 🧠 Memory | Aria | Persistent memory, user profile, context |

---

## Quick Start

### Prerequisites
- Docker + Docker Compose
- Anthropic API key
- Telegram Bot token (from [@BotFather](https://t.me/BotFather))

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/kiboru.git
cd kiboru
```

### 2. Configure environment
```bash
cp .env.example .env
# Edit .env with your API keys
nano .env
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
```

---

## Agent Packs (Coming Soon)

Agent packs are bundles of specialized agents for specific lifestyles:

- 🏃 **Healthy Life Pack** — workout scheduler, meal planner, habit tracker
- 🎬 **Creator Pack** — shoot schedule, video concepts, caption writer
- ◎ **Crypto Pack** — token monitor, wallet tracker, alpha research
- 📚 **Student Pack** — study schedule, research assistant, deadline tracker

Packs will be unlockable via $KIBORU token (coming soon).

---

## Community

- X: [@KiboruAI](https://x.com/KiboruAI)
- Telegram: [t.me/KiboruAI](https://t.me/KiboruAI)

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

*Built with ❤️ on OpenClaw*
