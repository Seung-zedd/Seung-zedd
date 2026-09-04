<img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=header&text=Seung-je's%20Github&fontSize=90" />

# Hi there, I'm Cho Seung-je! 👋
### Backend Engineer who builds AI systems that actually run in production — not just prototypes

<p align="left">
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white"/>
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white"/>
  <img src="https://img.shields.io/badge/Claude_Code-111111?style=flat-square"/>
</p>

## 🚀 About Me
Backend engineer focused on turning AI features into systems that survive real traffic — not just working demos.

I care about three things after implementation: **performance, failure modes, and operational cost**. I also use AI agents as part of the engineering workflow itself — delegating repeatable implementation and verification work while keeping architecture, security boundaries, and acceptance decisions under explicit human ownership.

- Reduced LLM API costs by **98%** through batching architecture and retry design
- Removed OOM risk by separating large-file processing from the JVM heap
- Improved a search API from **24.04s P95 to 2.014s**, then verified the root cause with `performance_schema`, `EXPLAIN`, and k6 instead of stopping at the first plausible hypothesis
- Built and documented an **AI-agent orchestration workflow** with SPECs, acceptance criteria, review loops, and human approval gates

## 🛠️ Technical Skills
- **Languages & Frameworks:** Java 21, Spring Boot, Spring Data JPA, QueryDSL, SvelteKit, TypeScript
- **Databases:** MySQL, PostgreSQL, pgvector
- **AI / Agentic Development:** LLM APIs, LangChain4j, Claude Code, MoAI-ADK, prompt / agent workflow design
- **Performance & Observability:** k6, Prometheus, Grafana, Micrometer, HikariCP, MySQL `performance_schema`
- **Infra & DevOps:** Docker, GitHub Actions, Vercel

## 📈 Featured Projects

### 🧠 [Cubrain](https://github.com/Seung-zedd/cubrain) — AI-powered PDF study SaaS
- Cut LLM API costs by **98%** through synthetic batching and exponential-backoff retry
- Reduced JVM heap pressure and OOM risk by spooling uploaded files to temporary disk storage
- Designed context extraction and SSE delivery to turn LLM output into an operable user-facing workflow

### ⚡ [sbb_board](https://github.com/Seung-zedd/sbb_board) — Backend performance engineering
- Reduced a 1:N lookup from **6,506ms → 70ms** using semi-join + Stream API mapping
- Under VU100 load, improved search P95 from **24.04s → 2.014s** and reduced the 3s SLO exceed rate to **0.44%**
- Tested the HikariCP saturation hypothesis by changing pool size and **discarded it when the data did not move**
- Traced the real bottleneck to an `OR` condition preventing FULLTEXT index use, then verified the rewrite with `EXPLAIN`, response-equivalence checks, regression tests, and k6

### 🎙️ [EchoBloom](https://github.com/Seung-zedd/echo-bloom-server) — AI-powered affirmation speaking service (team of 6)
- Implemented STT result normalization and Levenshtein-based similarity scoring
- Worked across API boundaries and service flows in a 6-person team project

### 🛡️ [secure-file-upload](https://github.com/Seung-zedd/secure-file-upload) — AI-agent orchestration + server-side upload validation
- Defined requirements and acceptance criteria first, then used **MoAI-ADK + Claude Code** to delegate implementation and verification work
- Kept human approval around architecture, security policy, secret handling, and other high-risk decisions
- Recorded **46 decision markers** in `PROMPT_LOG.md`: 24 accepted directly, 17 accepted after revision, 3 rejected, 2 deferred
- Of the 17 revised decisions, **11 were corrected by the AI verification loop itself and 6 required direct human intervention**
- The repository is intended as supporting evidence of **how I decide what to delegate to AI and what not to delegate**

---

## 🎮 Activities
- **Google Gemini 3 Hackathon — [Lucidify](https://github.com/Seung-zedd/lucidify):** Built a multimodal lucid-dreaming interface with SvelteKit and GCP serverless tooling within the hackathon window
- **AI 포텐데이 x Naver Cloud Hackathon:** Led backend + AI/STT integration for EchoBloom, shipping a full plan-to-release cycle in 20 days

---

📫 **How to reach me:**
- **LinkedIn:** [![My LinkedIn](https://img.shields.io/badge/LinkedIn%20Profile-SeungJe-blue?logo=data:image/svg%2bxml;base64,PHN2ZyByb2xlPSJpbWciIGZpbGw9IiNmZmZmZmYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+TGlua2VkSW48L3RpdGxlPjxwYXRoIGQ9Ik0yMC40NDcgMjAuNDUyaC0zLjU1NHYtNS41NjljMC0xLjMyOC0uMDI3LTMuMDM3LTEuODUyLTMuMDM3LTEuODUzIDAtMi4xMzYgMS40NDUtMi4xMzYgMi45Mzl2NS42NjdIOS4zNTFWOWgzLjQxNHYxLjU2MWguMDQ2Yy40NzctLjkgMS42MzctMS44NSAzLjM3LTEuODUgMy42MDEgMCA0LjI2NyAyLjM3IDQuMjY3IDUuNDU1djYuMjg2ek01LjMzNyA3LjQzM2MtMS4xNDQgMC0yLjA2My0uOTI2LTIuMDYzLTIuMDY1IDAtMS4xMzguOTItMi4wNjMgMi4wNjMgMS4xNCAwIDIuMDY0LjkyNSAyLjA2NCAyLjA2MyAwIDEuMTM5LS45MjUgMi4wNjUtMi4wNjQgMi4wNjV6bTEuNzgyIDEzLjAxOUgzLjU1NVY5aDMuNTY0djExLjQ1MnpNMjIuMjI1IDBIMS43NzFDLjc5MiAwIDAgLjc3NCAwIDEuNzI5djIwLjU0MkMwIDIzLjIyNy43OTIgMjQgMS43NzEgMjRoMjAuNDUxQzIzLjIgMjQgMjQgMjMuMjI3IDI0IDIyLjI3MVYxLjcyOUMyNCAuNzc0IDIzLjIgMCAyMi4yMjIgMGguMDAzeiIvPjwvc3ZnPgo=)](https://www.linkedin.com/in/seung-zedd/)
