<div align="center">

# 🎱 Soc Ops

**Social Bingo for in-person mixers — powered by GitHub Copilot Agent Mode**

*Find people who match the prompts. Get 5 in a row. Break the ice.*

[![Java 21](https://img.shields.io/badge/Java-21-orange?logo=openjdk&logoColor=white)](https://adoptium.net/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.4-brightgreen?logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![GitHub Copilot](https://img.shields.io/badge/Built%20with-GitHub%20Copilot-black?logo=github&logoColor=white)](https://github.com/features/copilot)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

---

### 🚀 [Start the Lab Guide →](workshop/GUIDE.md)

</div>

---

## What is this?

**Soc Ops** is a hands-on workshop disguised as a game. You'll take a working Social Bingo app and level it up using **VS Code Agent Mode** with GitHub Copilot — learning real-world agentic development skills along the way.

> 🕐 ~1 hour · 🎯 Intermediate · ☕ Java 21 / Spring Boot

---

## 🗺️ Lab Roadmap

| Part | Title | What you'll do |
|:----:|-------|----------------|
| [**00**](workshop/00-overview.md) | Overview & Checklist | Orient yourself and verify your setup |
| [**01**](workshop/01-setup.md) | Setup & Context Engineering | Clone, configure, and teach Copilot about your codebase |
| [**02**](workshop/02-design.md) | Design-First Frontend | Redesign the UI with creative AI-driven themes |
| [**03**](workshop/03-quiz-master.md) | Custom Quiz Master | Build a custom agent that generates bingo prompts |
| [**04**](workshop/04-multi-agent.md) | Multi-Agent Development | Ship new features with TDD + design agents in parallel |

> 📝 All guides are available offline in the [`workshop/`](workshop/) folder.

---

## 🎯 Skills You'll Build

| Skill | Description |
|-------|-------------|
| 🧠 **Context Engineering** | Teach AI about your codebase with `.github/copilot-instructions.md` |
| 🤖 **Agentic Primitives** | Use background agents, cloud agents, and custom workflows |
| 🎨 **Design-First Development** | Let AI iterate on UI while you guide the creative vision |
| 🧪 **Test-Driven Development** | Use TDD agents to build reliable features fast |

---

## ⚡ Quick Start

**Prerequisites:** [Java 21 JDK](https://adoptium.net/) · [Maven 3.9+](https://maven.apache.org/)

> 💡 **Tip:** Use the included [DevContainer](.devcontainer) for a zero-setup environment.

```bash
# Run
cd socops && ./mvnw spring-boot:run

# Build
cd socops && ./mvnw clean package

# Test
cd socops && ./mvnw test
```

Open [http://localhost:8080](http://localhost:8080) and start playing.

---

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Deploys automatically to GitHub Pages on push to `main`.
