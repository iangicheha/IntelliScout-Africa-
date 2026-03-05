# IntelliScout Africa 🌍
### AI-Powered Competitive Intelligence Platform for African B2B Companies

---

## What This Does
IntelliScout Africa is a multi-agent AI system that automatically monitors competitors 
for African B2B companies and delivers weekly intelligence reports via WhatsApp and email.

It replaces expensive human market research consultants with a 24/7 AI agent team.

---

## The 5 Agents

| Agent | Folder | Job |
|---|---|---|
| Orchestrator | /orchestrator | Manages and coordinates all agents |
| Collection Agent | /agents/collection | Scrapes competitor data from web, social, news |
| Signal Agent | /agents/signal | Detects what actually changed and matters |
| Report Agent | /agents/report | Writes the weekly intelligence brief |
| Alert Agent | /agents/alert | Fires instant WhatsApp alerts for urgent changes |
| Learning Agent | /agents/learning | Improves accuracy over time from feedback |

---

## Project Structure

```
intelliscout-africa/
├── main.py                  # Entry point
├── requirements.txt         # Python dependencies
├── .env.example             # Environment variables template
├── docker-compose.yml       # Run with one command
├── orchestrator/            # Master coordinator
├── agents/                  # The 5 specialist AI agents
│   ├── collection/          # Scrapes web, social, news
│   ├── signal/              # Detects what changed
│   ├── report/              # Writes intelligence brief
│   ├── alert/               # Fires real-time alerts
│   └── learning/            # Improves over time
├── shared/                  # Shared memory, utils, config
├── data/                    # Raw, processed, reports
├── delivery/                # WhatsApp + Email delivery
├── dashboard/               # Web dashboard (FastAPI)
└── tests/                   # Unit tests per agent
```

---

## Quick Start

```bash
git clone https://github.com/your-org/intelliscout-africa.git
cd intelliscout-africa
pip install -r requirements.txt
cp .env.example .env
docker-compose up -d redis
python main.py
```

---

## Environment Variables

```
ANTHROPIC_API_KEY=
WHATSAPP_API_TOKEN=
SENDGRID_API_KEY=
REDIS_URL=
DATABASE_URL=
```

Built for African B2B companies. Starting in Kenya. 🇰🇪
