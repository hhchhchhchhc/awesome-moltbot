# Awesome Moltbot Resources [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated collection of resources for Moltbot (OpenClaw) - the open-source personal AI agent framework. Documentation, tutorials, skills, security guides, and community resources.

**100,000+ GitHub Stars** | **2M+ Weekly Visitors** | **500+ Community Skills**

[English](#contents) | [中文](#中文版)

---

## What is Moltbot?

**Moltbot** (now **OpenClaw**) is an open-source, local-first AI agent framework that enables autonomous, 24/7 AI assistants. It connects to messaging platforms (Telegram, WhatsApp, Discord, Slack, Signal) and executes tasks using LLMs like Claude, GPT-4, Gemini, or local models.

### Name Evolution
| Date | Name | Reason |
|------|------|--------|
| Nov 2025 | Clawd / Clawdbot | Original name |
| Jan 2026 | Moltbot | Anthropic trademark request |
| Jan 29, 2026 | OpenClaw | Final rebranding |

### Key Features
- **Local-First Architecture** - Data stored on your device, full privacy control
- **Persistent Memory** - Remembers context across sessions via `MEMORY.md`
- **Multi-Channel** - Telegram, WhatsApp, Discord, Slack, Signal, Web
- **Extensible Skills** - 500+ community skills, create custom ones
- **Multi-Model Support** - Claude, GPT-4, Gemini, MiniMax, local models
- **MCP Protocol** - Standardized tool integration layer

---

## Contents

- [Official Resources](#official-resources)
- [Installation & Setup](#installation--setup)
- [Documentation](#documentation)
- [Architecture Deep Dive](#architecture-deep-dive)
- [Skills & Extensions](#skills--extensions)
- [Trading & DeFi Integration](#trading--defi-integration)
- [Security Best Practices](#security-best-practices)
- [Deployment Options](#deployment-options)
- [Tutorials & Guides](#tutorials--guides)
- [Community](#community)
- [Alternatives & Comparisons](#alternatives--comparisons)
- [Research & Articles](#research--articles)
- [Contributing](#contributing)

---

## Official Resources

### Core Links
| Resource | URL | Description |
|----------|-----|-------------|
| **Official Website** | [openclaw.ai](https://openclaw.ai) | Main website and documentation |
| **GitHub Repository** | [github.com/openclaw/openclaw](https://github.com/openclaw/openclaw) | Source code (100k+ stars) |
| **Blog** | [openclaw.ai/blog](https://openclaw.ai/blog/introducing-openclaw) | Official announcements |
| **Discord Community** | Discord | 8,900+ members |
| **MoltHub Skills** | [molthub.com](https://molthub.com) | Skills marketplace |

### Related Repositories
| Repository | Description | Verified |
|------------|-------------|----------|
| [openclaw/openclaw](https://github.com/openclaw/openclaw) | Main repository (149k+ stars) | Yes |
| [moltbot/moltbot](https://github.com/moltbot/moltbot) | Legacy Moltbot repository | Yes |
| [molt-bot](https://github.com/molt-bot) | Moltbot GitHub organization | Yes |
| [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) | Community skills collection | Yes |

### Additional Resources
| Resource | URL | Description |
|----------|-----|-------------|
| **Wikipedia** | [en.wikipedia.org/wiki/OpenClaw](https://en.wikipedia.org/wiki/OpenClaw) | Official Wikipedia page |
| **Railway Deploy** | [railway.com/deploy/openclaw](https://railway.com/deploy/openclaw-prev-clawdbot-moltbot-self-host) | One-click Railway deployment |
| **Home Assistant** | [community.home-assistant.io](https://community.home-assistant.io/t/openclaw-clawdbot-on-home-assistant/981467) | Home Assistant integration |

**Sources:** [OpenClaw Official Blog](https://openclaw.ai/blog/introducing-openclaw) | [Wikipedia](https://en.wikipedia.org/wiki/OpenClaw) | [Vertu News](https://vertu.com/ai-tools/openclaw-achieves-100k-github-stars-after-third-rebrand-the-lobsters-final-evolution/) | [Trending Topics EU](https://www.trendingtopics.eu/openclaw-2-million-visitors-in-a-week/)

---

## Installation & Setup

### Quick Install (One Command)
```bash
# Official installer (handles all dependencies)
curl -fsSL https://openclaw.ai/install.sh | bash

# Alternative (legacy)
curl -fsSL https://clawd.bot/install.sh | bash
```

### Manual Installation
```bash
# Prerequisites: Node.js 22+, npm
npm install -g moltbot@latest

# Start setup wizard
moltbot setup
```

### Migration from Clawdbot
```bash
# Uninstall old version
npm uninstall -g clawdbot

# Install new version
npm install -g moltbot@latest

# Run migration wizard
moltbot migrate
```

### Setup Wizard Steps
1. **Choose AI Provider** - Anthropic, OpenAI, MiniMax, OpenRouter, Local
2. **Enter API Key** - Your provider's API key
3. **Select Default Model** - Claude Opus 4.5 (default), GPT-4o, Gemini 3 Pro
4. **Connect Channel** - Telegram, WhatsApp, Discord, etc.
5. **Configure Skills** - Select initial skill set
6. **Enable Memory Hook** - Persistent memory across sessions
7. **Hatch Your Bot** - Give it an identity and launch

### Channel-Specific Setup

#### Telegram
```
1. Open Telegram → Search @BotFather
2. Send /newbot → Choose name and username (ending in "bot")
3. Copy API token → Paste into Moltbot terminal
4. Start chat with your bot → Send /start
5. Enter pairing code in terminal
```

#### WhatsApp
```
1. Ask Moltbot: "Help me connect my WhatsApp"
2. Open Channels → Select WhatsApp
3. Click "Show QR" → Scan with WhatsApp app
4. Enter phone number with country code
```

**Sources:** [Datacamp Tutorial](https://www.datacamp.com/tutorial/moltbot-clawdbot-tutorial) | [Young Urban Project Guide](https://www.youngurbanproject.com/moltbot-setup-guide-clawdbot/) | [Codecademy Article](https://www.codecademy.com/article/open-claw-tutorial-installation-to-first-chat-setup)

---

## Documentation

### Official Documentation
| Resource | Platform | Focus |
|----------|----------|-------|
| [DigitalOcean Docs](https://docs.digitalocean.com/products/marketplace/catalog/moltbot/) | DigitalOcean | Deployment guide |
| [DigitalOcean Quickstart](https://www.digitalocean.com/community/tutorials/moltbot-quickstart-guide) | DigitalOcean | Getting started |
| [MiniMax Integration](https://platform.minimax.io/docs/solutions/moltbot) | MiniMax | Model integration |
| [Emergent Tutorial](https://emergent.sh/tutorial/moltbot-on-emergent) | Emergent | Cloud deployment |
| [API Yi Guide](https://help.apiyi.com/en/clawdbot-renamed-moltbot-complete-guide-en.html) | API Yi | Complete guide |

### Community Guides
| Guide | Author/Platform | Topic |
|-------|-----------------|-------|
| [Ultimate Guide to OpenClaw](https://www.reddit.com/r/ThinkingDeeplyAI/comments/1qsoq4h/the_ultimate_guide_to_openclaw_formerly_clawdbot/) | Reddit | Comprehensive overview |
| [Memory Architecture Guide](https://zenvanriel.nl/ai-engineer-blog/moltbot-memory-architecture-guide/) | Zen van Riel | Memory system deep dive |
| [Custom Skill Creation](https://zenvanriel.nl/ai-engineer-blog/moltbot-custom-skill-creation-guide/) | Zen van Riel | Building custom skills |
| [Channel Comparison](https://zenvanriel.nl/ai-engineer-blog/moltbot-channel-comparison-telegram-whatsapp-signal/) | Zen van Riel | Telegram vs WhatsApp vs Signal |
| [What is OpenClaw](https://www.digitalocean.com/resources/articles/what-is-openclaw) | DigitalOcean | Conceptual overview |

**Sources:** [DigitalOcean Catalog](https://docs.digitalocean.com/products/marketplace/catalog/moltbot/) | [Reddit Guide](https://www.reddit.com/r/ThinkingDeeplyAI/comments/1qsoq4h/the_ultimate_guide_to_openclaw_formerly_clawdbot/)

---

## Architecture Deep Dive

### System Architecture
```
┌─────────────────────────────────────────────────────────────────┐
│                         MOLTBOT ARCHITECTURE                     │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│   ┌──────────────┐     ┌──────────────┐     ┌──────────────┐   │
│   │   Telegram   │     │   WhatsApp   │     │   Discord    │   │
│   │   Channel    │     │   Channel    │     │   Channel    │   │
│   └──────┬───────┘     └──────┬───────┘     └──────┬───────┘   │
│          │                    │                    │            │
│          └────────────────────┼────────────────────┘            │
│                               ▼                                  │
│                    ┌──────────────────┐                         │
│                    │  Gateway (Local) │                         │
│                    │  - Routing       │                         │
│                    │  - Context       │                         │
│                    │  - Permissions   │                         │
│                    └────────┬─────────┘                         │
│                             │                                    │
│          ┌──────────────────┼──────────────────┐                │
│          ▼                  ▼                  ▼                │
│   ┌────────────┐    ┌────────────┐    ┌────────────┐           │
│   │   Memory   │    │   Skills   │    │    LLM     │           │
│   │  System    │    │   Engine   │    │   Backend  │           │
│   └────────────┘    └────────────┘    └────────────┘           │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

### Memory System (Local-First)

| Component | File | Purpose |
|-----------|------|---------|
| **Daily Logs** | `memory/YYYY-MM-DD.md` | Append-only interaction logs |
| **Long-Term Memory** | `MEMORY.md` | Curated preferences & decisions |
| **Boot Configuration** | `boot.md` | Startup rules and context |

#### Memory Retrieval
- **Semantic Search** - Vector embeddings for similarity matching
- **Keyword Search** - BM25 algorithm for exact matches
- **Hybrid Approach** - Combines both for optimal retrieval

#### Memory Flush
Automatic preservation before context compaction ensures no critical information is lost.

### Hooks System
| Hook | Purpose | Example |
|------|---------|---------|
| `boot-md` | Load startup context | Inject rules/preferences |
| `pre-response` | Modify before sending | Content filtering |
| `post-action` | Execute after task | Logging, notifications |

**Sources:** [Memory Architecture Article](https://medium.com/aimonks/clawdbots-memory-architecture-pre-compaction-flush-the-engineering-reality-behind-never-c8ff84a4a11a) | [Tencent Cloud Techpedia](https://www.tencentcloud.com/techpedia/136811)

---

## Skills & Extensions

### What are Skills?
Skills are instruction files (`SKILL.md`) that teach Moltbot how to use specific tools. They're packaged as ZIP files containing:
- Markdown instructions
- Scripts and configurations
- Tool definitions

### Installing Skills
```bash
# From MoltHub
npx molthub@latest install <skill-name>

# From local file
moltbot skill install ./my-skill.zip

# List installed skills
moltbot skills list
```

### Skill Categories (500+ Available)

| Category | Examples | Count |
|----------|----------|-------|
| **Development** | Git, Docker, CI/CD, Code Review | 50+ |
| **Trading & Finance** | Hyperliquid, DeFi, Polymarket | 30+ |
| **Productivity** | Email, Calendar, Notes, Tasks | 40+ |
| **Browser Automation** | Web scraping, Form filling | 25+ |
| **Smart Home** | IoT control, Automation | 20+ |
| **Social Media** | Twitter/X, LinkedIn, Content | 35+ |
| **Data & Analytics** | SQL, Visualization, Reports | 30+ |
| **Communication** | Slack, Teams, Messaging | 25+ |

### Skill Resources
| Resource | URL | Description | Verified |
|----------|-----|-------------|----------|
| MoltDirectory | [Reddit Post](https://www.reddit.com/r/LocalLLM/comments/1qq32b4/resource_500_formatted_skills_for_moltbotclawdbot/) | 500+ pre-built skills | Yes |
| Awesome OpenClaw Skills | [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) | Community curated skills | Yes |
| Community Skills | [r/LocalLLM](https://www.reddit.com/r/LocalLLM/) | User-contributed skills | Yes |
| Skills SaaS Directory | [Reddit SaaS](https://www.reddit.com/r/SaaS/comments/1qpodoh/i_opensourced_a_directory_of_500_skills_for/) | Open-sourced directory | Yes |

### Creating Custom Skills
```markdown
# SKILL.md Template

## Skill Name
Description of what this skill does

## Tools Required
- Tool 1: Description
- Tool 2: Description

## Instructions
1. Step-by-step guide for the agent
2. How to use the tools
3. Expected outputs

## Examples
- Example input → Expected output
```

**Sources:** [Microsoft Tech Community](https://techcommunity.microsoft.com/blog/appsonazureblog/%F0%9F%A6%9E-deploy-moltbot-to-azure-container-apps-your-247-ai-assistant-in-30-minutes/4490611) | [Reddit Skills Directory](https://www.reddit.com/r/SaaS/comments/1qpodoh/i_opensourced_a_directory_of_500_skills_for/)

---

## Trading & DeFi Integration

### Hyperliquid Integration
Moltbot can integrate with Hyperliquid for automated perpetual futures trading.

```python
# Example: Hyperliquid API setup
from hyperliquid.info import Info
from hyperliquid.exchange import Exchange

# Initialize with API credentials
info = Info()
exchange = Exchange(wallet, api_url)

# Place orders programmatically
order = exchange.order(
    coin="BTC",
    is_buy=True,
    sz=0.01,
    limit_px=50000,
    order_type={"limit": {"tif": "Gtc"}}
)
```

### Trading Use Cases
| Use Case | Description |
|----------|-------------|
| **Market Monitoring** | 24/7 price alerts and condition tracking |
| **Strategy Execution** | Automated trading based on signals |
| **Portfolio Rebalancing** | Periodic adjustment of positions |
| **News-Driven Trading** | React to market news automatically |
| **Risk Management** | Stop-loss and take-profit automation |

### DeFi & Web3 Automation
| Protocol | Integration |
|----------|-------------|
| **Polymarket** | Prediction market trading |
| **Uniswap/DEXs** | Token swaps, liquidity provision |
| **Aave/Compound** | Lending/borrowing automation |
| **NFT Platforms** | Minting, trading, monitoring |

### Trading Skills
| Skill | Description |
|-------|-------------|
| `hyperliquid-trader` | Perpetual futures trading |
| `polymarket-bot` | Prediction market automation |
| `defi-monitor` | Protocol TVL and yield tracking |
| `whale-watcher` | Large transaction alerts |
| `funding-rate-arb` | Funding rate arbitrage |

**Sources:** [Phemex News](https://phemex.com/news/article/moltbot-emerges-as-a-key-ai-tool-for-web3-automation-57168) | [Wundertrading Guide](https://wundertrading.com/journal/en/learn/article/hyperliquid-api-trading-bot)

---

## Security Best Practices

### Risk Overview
Moltbot's power comes with significant security considerations. The "lethal trifecta" of risks:

1. **Access to Private Data** - Emails, files, messages
2. **Exposure to Untrusted Inputs** - Web content, messages from strangers
3. **External Communication** - Can send data outward

### OWASP Top 10 for Agentic AI
| Risk | Description | Mitigation |
|------|-------------|------------|
| **Prompt Injection** | Malicious instructions via inputs | Input sanitization, sandboxing |
| **Sensitive Data Exposure** | Leaking private information | Encryption, access controls |
| **Insecure Skill Execution** | Malicious skill packages | Audit skills, disable auto-install |
| **Excessive Permissions** | Over-privileged agent | Least-privilege configuration |
| **Lack of Monitoring** | Undetected malicious activity | Verbose logging, alerting |

### Security Hardening Checklist

#### Infrastructure
- [ ] Run in isolated VM or container
- [ ] Use Docker with minimal privileges
- [ ] Block outbound access except approved endpoints
- [ ] Never expose on public internet
- [ ] Use reverse-proxy with authentication
- [ ] Implement IP whitelisting

#### Configuration
- [ ] Disable shell execution when not needed
- [ ] Restrict file system paths
- [ ] Use API key rotation
- [ ] Encrypt secrets at rest
- [ ] Enable Docker sandboxing

#### Skills Management
- [ ] Manually review `SKILL.md` before install
- [ ] Avoid auto-install of skills
- [ ] Source skills from vetted repositories only
- [ ] Wait for community audits on new skills
- [ ] Disable unnecessary tool access

#### Monitoring
- [ ] Enable verbose logging
- [ ] Set up endpoint detection
- [ ] Alert on outbound traffic spikes
- [ ] Monitor directories for anomalies
- [ ] Regular security audits

### Secure Deployment Example
```yaml
# docker-compose.yml (hardened)
version: '3.8'
services:
  moltbot:
    image: openclaw/moltbot:latest
    security_opt:
      - no-new-privileges:true
    read_only: true
    tmpfs:
      - /tmp
    networks:
      - moltbot-internal
    environment:
      - SHELL_EXECUTION=disabled
      - FILE_PATH_RESTRICTION=/app/workspace
```

**Sources:** [Forbes Article](https://www.forbes.com/sites/ronschmelzer/2026/01/30/moltbot-molts-again-and-becomes-openclaw-pushback-and-concerns-grow/) | [Palo Alto Networks Blog](https://www.paloaltonetworks.com/blog/network-security/why-moltbot-may-signal-ai-crisis/) | [Snyk Security Guide](https://snyk.io/articles/clawdbot-ai-assistant/) | [Ken Huang Substack](https://kenhuangus.substack.com/p/moltbook-security-risks-in-ai-agent)

---

## Deployment Options

### One-Click Deployments
| Platform | Link | Features |
|----------|------|----------|
| **DigitalOcean** | [Marketplace](https://docs.digitalocean.com/products/marketplace/catalog/moltbot/) | 1-Click, Ubuntu 24.04, Docker |
| **Azure Container Apps** | [Tutorial](https://techcommunity.microsoft.com/blog/appsonazureblog/%F0%9F%A6%9E-deploy-moltbot-to-azure-container-apps-your-247-ai-assistant-in-30-minutes/4490611) | 30-min setup, scalable |
| **Zeabur** | [Template](https://zeabur.com/templates/VTZ4FX) | Easy cloud deployment |
| **Emergent** | [Tutorial](https://emergent.sh/tutorial/moltbot-on-emergent) | Managed runtime |

### Self-Hosted Options
| Option | Best For | Complexity |
|--------|----------|------------|
| **Local Machine** | Development, testing | Low |
| **Raspberry Pi** | Always-on, low cost | Medium |
| **VPS (Hetzner, Vultr)** | Production, reliability | Medium |
| **Docker Compose** | Reproducible setup | Medium |
| **Kubernetes** | Enterprise, scaling | High |

### Hardware Requirements
| Component | Minimum | Recommended |
|-----------|---------|-------------|
| CPU | 2 cores | 4+ cores |
| RAM | 4 GB | 8+ GB |
| Storage | 20 GB SSD | 50+ GB SSD |
| Network | 10 Mbps | 100+ Mbps |

---

## Tutorials & Guides

### Video Tutorials
| Title | Platform | Duration |
|-------|----------|----------|
| [Complete ClawdBot Tutorial](https://vertu.com/lifestyle/complete-clawdbot-tutorial-deploy-with-caution/) | Vertu | Long-form |
| [Moltbot Setup Guide](https://www.youngurbanproject.com/moltbot-setup-guide-clawdbot/) | Young Urban Project | Beginner |

### Written Tutorials
| Tutorial | Platform | Level |
|----------|----------|-------|
| [Datacamp Tutorial](https://www.datacamp.com/tutorial/moltbot-clawdbot-tutorial) | Datacamp | Beginner |
| [Dev.to Ultimate Guide](https://dev.to/czmilo/moltbot-the-ultimate-personal-ai-assistant-guide-for-2026-d4e) | Dev.to | Intermediate |
| [MCPs & Moltbot Workflow](https://dev.to/austinwdigital/mcps-claude-code-codex-moltbot-clawdbot-and-the-2026-workflow-shift-in-ai-development-1o04) | Dev.to | Advanced |
| [Analytics Vidhya Moltbook](https://www.analyticsvidhya.com/blog/2026/02/moltbook-for-openclaw-agents/) | Analytics Vidhya | Intermediate |
| [Safety Lessons](https://www.aicerts.ai/news/prompt-engineering-safety-lessons-from-moltbots-viral-storm/) | AICerts | Security |

### Use Case Guides
| Use Case | Description |
|----------|-------------|
| Stock Monitoring | 24/7 market tracking with alerts |
| PR Review Automation | Auto-review GitHub pull requests |
| Content Publishing | Cross-platform content management |
| Wine Cellar Tracking | Custom inventory management |
| Email Assistant | Smart email triage and responses |

**Sources:** [Vertu Tutorial](https://vertu.com/lifestyle/complete-clawdbot-tutorial-deploy-with-caution/) | [Datacamp](https://www.datacamp.com/tutorial/moltbot-clawdbot-tutorial)

---

## Community

### Official Channels
| Platform | Link | Members |
|----------|------|---------|
| **Discord** | Official Server | 8,900+ |
| **GitHub Discussions** | [openclaw/openclaw](https://github.com/openclaw/openclaw) | Active |
| **Reddit** | r/ThinkingDeeplyAI | Growing |

### Community Resources
| Resource | Description |
|----------|-------------|
| [r/LocalLLM](https://www.reddit.com/r/LocalLLM/) | Local AI discussions |
| [r/SaaS Skills Directory](https://www.reddit.com/r/SaaS/comments/1qpodoh/i_opensourced_a_directory_of_500_skills_for/) | Community skills |

### Getting Help
1. **Discord** - Real-time community support
2. **GitHub Issues** - Bug reports and feature requests
3. **Documentation** - Official guides
4. **Stack Overflow** - Tag: `moltbot` or `openclaw`

---

## Alternatives & Comparisons

### Comparison Matrix
| Feature | Moltbot/OpenClaw | ChatGPT | Claude | Manus | Saner.AI |
|---------|------------------|---------|--------|-------|----------|
| **Open Source** | Yes | No | No | No | No |
| **Self-Hosted** | Yes | No | No | Yes | No |
| **Local-First** | Yes | No | No | No | No |
| **Persistent Memory** | Yes | Limited | Limited | Yes | Yes |
| **Multi-Channel** | Yes | No | No | No | No |
| **Custom Skills** | 500+ | Plugins | MCP | Limited | No |
| **24/7 Autonomous** | Yes | No | No | Yes | Yes |

### Alternative Tools
| Tool | Best For | Key Difference |
|------|----------|----------------|
| [Saner.AI](https://www.saner.ai/blogs/best-moltbot-clawdbot-alternatives) | Personal productivity | Simpler, less autonomous |
| [Knolli.ai](https://www.knolli.ai/post/clawdbot-alterantive) | Enterprise teams | Scoped permissions, security focus |
| [Manus](https://manus.ai) | Workflow automation | Closed source, managed |
| [LangChain Agents](https://langchain.com) | Developers | Framework, not product |
| [AutoGPT](https://github.com/Significant-Gravitas/AutoGPT) | Experimentation | Less polished |

**Sources:** [Saner.AI Blog](https://www.saner.ai/blogs/best-moltbot-clawdbot-alternatives) | [Knolli Comparison](https://www.knolli.ai/post/clawdbot-alterantive) | [SourceForge Comparison](https://sourceforge.net/software/compare/Claude-Cowork-vs-OpenClaw/)

---

## Research & Articles

### News Coverage
| Article | Source | Date | Verified |
|---------|--------|------|----------|
| [Moltbot Molts Again and Becomes OpenClaw](https://www.forbes.com/sites/ronschmelzer/2026/01/30/moltbot-molts-again-and-becomes-openclaw-pushback-and-concerns-grow/) | Forbes | Jan 2026 | Yes |
| [Why Moltbot May Signal AI Crisis](https://www.paloaltonetworks.com/blog/network-security/why-moltbot-may-signal-ai-crisis/) | Palo Alto Networks | Jan 2026 | Yes |
| [OpenClaw Achieves 100k GitHub Stars](https://vertu.com/ai-tools/openclaw-achieves-100k-github-stars-after-third-rebrand-the-lobsters-final-evolution/) | Vertu | Jan 2026 | Yes |
| [OpenClaw: 2 Million Visitors in a Week](https://www.trendingtopics.eu/openclaw-2-million-visitors-in-a-week/) | Trending Topics | Jan 2026 | Yes |
| [Personal AI Agents Like OpenClaw Are a Security Nightmare](https://blogs.cisco.com/ai/personal-ai-agents-like-openclaw-are-a-security-nightmare) | Cisco | 2026 | Yes |
| [Moltbot Open Source AI Security Risks](https://cybernews.com/security/moltbot-open-source-ai-security-risks/) | CyberNews | 2026 | Yes |
| [OpenClaw Bug Enables One-Click RCE](https://thehackernews.com/2026/02/openclaw-bug-enables-one-click-remote.html) | The Hacker News | Feb 2026 | Yes |
| [What is OpenClaw/Moltbot](https://coinmarketcap.com/academy/article/what-is-openclaw-moltbot-clawdbot-ai-agent-crypto-twitter) | CoinMarketCap | 2026 | Yes |
| [ClawdBot: Not a ChatGPT Alternative](https://vertu.com/lifestyle/clawdbot-not-a-chatgpt-alternative-but-your-7x24-digital-employee/) | Vertu | 2025 | Yes |

### Technical Analysis
| Article | Source | Focus | Verified |
|---------|--------|-------|----------|
| [Memory Architecture Deep Dive](https://medium.com/aimonks/clawdbots-memory-architecture-pre-compaction-flush-the-engineering-reality-behind-never-c8ff84a4a11a) | AI Monks (Medium) | Memory system | Yes |
| [Security Risks in AI Agents](https://kenhuangus.substack.com/p/moltbook-security-risks-in-ai-agent) | Ken Huang (Substack) | Security analysis | Yes |
| [Clawdbot Renamed Moltbot Guide](https://help.apiyi.com/en/clawdbot-renamed-moltbot-complete-guide-en.html) | API Yi | Migration guide | Yes |
| [Moltbook Inside the AI-Only Social Network](https://medium.com/@adnanmasood/moltbook-inside-the-ai-only-social-network-that-has-everyone-talking-5e53613593ff) | Medium | Moltbook ecosystem | Yes |
| [OpenClaw (fka Moltbot, fka Clawdbot)](https://www.news.aakashg.com/p/openclaw-fka-moltbot-fka-clawdbot) | Aakash G Newsletter | History overview | Yes |
| [Clawdbot is Dead, Long Live Moltbot](https://levelup.gitconnected.com/clawdbot-is-dead-long-live-moltbot-5dc6a527312c) | Git Connected | Transition story | Yes |
| [Moltbot for OpenClaw Agents](https://www.analyticsvidhya.com/blog/2026/02/moltbook-for-openclaw-agents/) | Analytics Vidhya | Integration guide | Yes |

### Chinese Coverage (中文报道)
| Article | Source | Verified |
|---------|--------|----------|
| [创业邦报道](https://m.cyzone.cn/article/823301.html) | 创业邦 | Yes |
| [网易新闻](https://www.163.com/dy/article/KKFJB56305500HK7.html) | 网易 | Yes |
| [53AI分析](https://www.53ai.com/news/OpenSourceLLM/2026012949568.html) | 53AI | Yes |
| [36氪报道](https://eu.36kr.com/en/p/3661357114942337) | 36氪 | Yes |

---

## Contributing

Contributions are welcome! Please follow these guidelines:

### How to Contribute
1. Fork this repository
2. Create a feature branch (`git checkout -b add-resource`)
3. Add your resource in the appropriate section
4. Ensure links are valid and sources are credible
5. Submit a Pull Request

### Contribution Guidelines
- **Verify all links** before submitting
- **Include source URLs** for traceability
- **Use consistent formatting** (tables, markdown)
- **Add descriptions** that are informative
- **Avoid duplicates** - check existing content first

### What We're Looking For
- New tutorials and guides
- Community skills and extensions
- Security research and best practices
- Deployment configurations
- Integration examples
- Translations

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under CC0 1.0 Universal (Public Domain).

---

# 中文版

> Moltbot (OpenClaw) 资源精选 - 开源个人 AI Agent 框架的文档、教程、技能、安全指南和社区资源

## 什么是 Moltbot?

**Moltbot**（现更名为 **OpenClaw**）是一个开源的、本地优先的 AI Agent 框架，支持 24/7 自主运行的 AI 助手。它可以连接多种消息平台（Telegram、WhatsApp、Discord、Slack、Signal），并使用 Claude、GPT-4、Gemini 等大语言模型执行任务。

### 名称演变
| 时间 | 名称 | 原因 |
|------|------|------|
| 2025年11月 | Clawd / Clawdbot | 原始名称 |
| 2026年1月 | Moltbot | Anthropic 商标要求 |
| 2026年1月29日 | OpenClaw | 最终更名 |

### 核心特性
- **本地优先架构** - 数据存储在本地设备，完全隐私控制
- **持久化记忆** - 通过 `MEMORY.md` 跨会话记忆上下文
- **多渠道支持** - Telegram、WhatsApp、Discord、Slack、Signal、Web
- **可扩展技能** - 500+ 社区技能，支持自定义
- **多模型支持** - Claude、GPT-4、Gemini、MiniMax、本地模型
- **MCP 协议** - 标准化工具集成层

---

## 目录

- [官方资源](#官方资源)
- [安装与设置](#安装与设置)
- [文档资源](#文档资源)
- [架构详解](#架构详解)
- [技能与扩展](#技能与扩展)
- [交易与 DeFi 集成](#交易与-defi-集成)
- [安全最佳实践](#安全最佳实践)
- [部署选项](#部署选项)
- [教程与指南](#教程与指南)
- [社区资源](#社区资源)

---

## 官方资源

| 资源 | 链接 | 描述 |
|------|------|------|
| **官方网站** | [openclaw.ai](https://openclaw.ai) | 主站和文档 |
| **GitHub 仓库** | [github.com/openclaw/openclaw](https://github.com/openclaw/openclaw) | 源代码 (100k+ stars) |
| **Discord 社区** | Discord | 8,900+ 成员 |
| **技能市场** | [molthub.com](https://molthub.com) | MoltHub 技能库 |

---

## 安装与设置

### 快速安装
```bash
# 官方安装器（自动处理依赖）
curl -fsSL https://openclaw.ai/install.sh | bash
```

### 设置向导步骤
1. **选择 AI 提供商** - Anthropic、OpenAI、MiniMax、OpenRouter
2. **输入 API Key** - 对应提供商的密钥
3. **选择默认模型** - Claude Opus 4.5（默认）、GPT-4o、Gemini 3 Pro
4. **连接渠道** - Telegram、WhatsApp、Discord 等
5. **配置技能** - 选择初始技能集
6. **启用记忆钩子** - 跨会话持久记忆
7. **孵化机器人** - 设置身份并启动

---

## 架构详解

### 记忆系统（本地优先）

| 组件 | 文件 | 用途 |
|------|------|------|
| **日志** | `memory/YYYY-MM-DD.md` | 追加式交互日志 |
| **长期记忆** | `MEMORY.md` | 精选偏好和决策 |
| **启动配置** | `boot.md` | 启动规则和上下文 |

### 记忆检索
- **语义搜索** - 向量嵌入相似度匹配
- **关键词搜索** - BM25 算法精确匹配
- **混合方式** - 结合两者以优化检索

---

## 技能与扩展

### 技能分类（500+ 可用）

| 分类 | 示例 | 数量 |
|------|------|------|
| **开发工具** | Git、Docker、CI/CD、代码审查 | 50+ |
| **交易金融** | Hyperliquid、DeFi、Polymarket | 30+ |
| **生产力** | 邮件、日历、笔记、任务 | 40+ |
| **浏览器自动化** | 网页抓取、表单填写 | 25+ |
| **智能家居** | IoT 控制、自动化 | 20+ |

### 安装技能
```bash
# 从 MoltHub 安装
npx molthub@latest install <技能名>

# 列出已安装技能
moltbot skills list
```

---

## 交易与 DeFi 集成

### 交易用例
| 用例 | 描述 |
|------|------|
| **市场监控** | 24/7 价格警报和条件追踪 |
| **策略执行** | 基于信号的自动交易 |
| **投资组合再平衡** | 定期调整仓位 |
| **新闻驱动交易** | 自动响应市场新闻 |
| **风险管理** | 止损止盈自动化 |

### DeFi 与 Web3 自动化
| 协议 | 集成 |
|------|------|
| **Polymarket** | 预测市场交易 |
| **Uniswap/DEXs** | 代币交换、流动性提供 |
| **Aave/Compound** | 借贷自动化 |
| **NFT 平台** | 铸造、交易、监控 |

---

## 安全最佳实践

### 风险概述
Moltbot 的强大能力伴随着重大安全考量。"致命三角"风险：

1. **访问私有数据** - 邮件、文件、消息
2. **暴露于不可信输入** - 网页内容、陌生人消息
3. **外部通信能力** - 可向外发送数据

### 安全加固清单

#### 基础设施
- [ ] 在隔离的 VM 或容器中运行
- [ ] 使用最小权限的 Docker
- [ ] 除批准的端点外阻止出站访问
- [ ] 永不暴露在公网
- [ ] 使用反向代理认证
- [ ] 实施 IP 白名单

#### 技能管理
- [ ] 安装前手动审查 `SKILL.md`
- [ ] 避免自动安装技能
- [ ] 仅从可信仓库获取技能
- [ ] 等待社区审计新技能

---

## 部署选项

### 一键部署
| 平台 | 链接 | 特点 |
|------|------|------|
| **DigitalOcean** | [Marketplace](https://docs.digitalocean.com/products/marketplace/catalog/moltbot/) | 一键部署、Ubuntu 24.04、Docker |
| **Azure** | [教程](https://techcommunity.microsoft.com/blog/appsonazureblog/%F0%9F%A6%9E-deploy-moltbot-to-azure-container-apps-your-247-ai-assistant-in-30-minutes/4490611) | 30分钟设置、可扩展 |
| **Zeabur** | [模板](https://zeabur.com/templates/VTZ4FX) | 简易云部署 |

---

## 社区资源

### 官方渠道
| 平台 | 成员数 |
|------|--------|
| **Discord** | 8,900+ |
| **GitHub Discussions** | 活跃 |
| **Reddit** | r/ThinkingDeeplyAI |

### 中文报道
| 文章 | 来源 |
|------|------|
| [AI Agent 的崛起](https://m.cyzone.cn/article/823301.html) | 创业邦 |
| [开源 AI 助手深度解析](https://www.163.com/dy/article/KKFJB56305500HK7.html) | 网易 |
| [Moltbot 技术架构分析](https://www.53ai.com/news/OpenSourceLLM/2026012949568.html) | 53AI |

---

<div align="center">

**如果觉得有用，请 Star 支持！欢迎贡献资源！**

朋友们现在的Tardis API是solo 1200每月的档位，年付年付！（14400美元折合人民币10万多人民币）
现货、期货、期权的数据都有啦！需要数据的联系微信a13479004101，代下载每一T收费249，单次最低99。

致富证券可能是一张内地身份证5分钟线上开户美港股的最后一台车了。
开户奖励很丰厚，总价值高达HK$8,800，包括现金券、返现、股票和转仓回赠。推荐好友还能额外拿钱，上不封顶。具体奖励有：1. 开户直接拿HK$200现金券+交易券；2. 入金最高返HK$1,300，还送NVIDIA股票；3. 转仓最高回赠HK$7,000；4. 推荐好友每成功一个得HK$300。

注意需要通过我的邀请码XC6774（二维码：https://image2url.com/r2/default/images/1770021823559-f8b6c7cb-d63d-4b01-9ead-48455da15c08.png或者https://mp.weixin.qq.com/s/NnIA1hszlLCyQ6BVxTmMAw）注册才有数千额外奖励QAQ。

致富支持大陆用户无港卡开户 ，可尝试用工商银行等快速入金，需开户7天内入金1万港币等值的前才有上述奖励。

致富chief.apk
链接: https://pan.baidu.com/s/1gpI4JSYY6MwZqP8Ywor9Tw?pwd=hmec 提取码: hmec

![32ed3917f1f7f20f3e561e3b386da68e](https://github.com/user-attachments/assets/e6ad42c2-3bd1-4426-a4ac-53458cf2ce84)
![f2ded2c901a4e731b32d4addcce25f3c](https://github.com/user-attachments/assets/10d5fefd-a939-435a-b252-ec29f2bbbbea)
![微信图片_20260203141110_215_152](https://github.com/user-attachments/assets/bced6473-80cd-4569-9d20-44c46ffde382)
![微信图片_20260203141111_216_152](https://github.com/user-attachments/assets/320f2928-8201-4977-b81d-9dd47f94c48f)
</div>
