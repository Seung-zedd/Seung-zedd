
<img src="https://capsule-render.vercel.app/api?type=waving&amp;color=auto&amp;height=200&amp;section=header&amp;text=Seung-je's%20Github&amp;fontSize=90" />

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
</p>

## 🚀 About Me
Backend engineer focused on turning AI features into systems that survive real traffic — not just working demos.
Reduced LLM API costs by 98% through batch processing architecture, eliminated OOM failures via disk-spooling design,
and drove a search API from a 24s P95 under load down to sub-2s while closing out a full k6 threshold suite through
root-cause investigation (not guesswork)

## 🛠️ Technical Skills
- **Languages & Frameworks:** Java 21, Spring Boot, Spring Data JPA, QueryDSL
- **Databases:** MySQL, PostgreSQL, pgvector
- **AI/Infra:** LangChain4j, Firebase Auth, SSE, Local Disk Spooling
- **Performance & Observability:** k6, Prometheus, Grafana, Micrometer, HikariCP tuning
- **DevOps:** Docker, GitHub Actions

## 📈 Featured Projects

### 🧠 [Cubrain](https://github.com/Seung-zedd/cubrain) — AI-powered PDF study SaaS (live service)
- Cut LLM API costs by **98%** via page-level synthesis batching + exponential backoff retry
- Eliminated OOM failures (**0% failure rate**) with a local disk-spooling architecture (O(N) → O(1) heap)
- Designed a 3-tier context pipeline (Micro/Local/Macro) to suppress LLM hallucination

### ⚡ [sbb_board](https://github.com/Seung-zedd/sbb_board) — High-traffic backend performance engineering
- Resolved a Cartesian-product bottleneck via semi-join + Stream API mapping (**6,506ms → 70ms**, 98.9%)
- Cut search P95 by 91% via covering + FULLTEXT indexing (**24.04s → 2.18s**), but threshold still failed at 51.58%
- Hypothesized connection-pool saturation, tested it directly (pool ×1/×2/×4) — **disproved it** by observed data
- Traced the real cause to an `OR` clause silently disabling the FULLTEXT index; rewrote via UNION + derived-table JOIN
- Verified via EXPLAIN + 15-case response-hash equality + 8 regression tests, then closed all 3 k6 thresholds (**0.44% error rate**)

### 🎙️ [EchoBloom](https://github.com/Seung-zedd/EchoBloom) — AI-powered affirmation speaking service (team, 6 members)
- Cut pronunciation-feedback latency by 99.9% (3,800ms → 2ms) via Korean text normalization + Levenshtein DP
- Improved scoring accuracy reliability by 15% by filtering out STT misrecognition noise before scoring

---

## 🎮 Activities
- **Google Gemini 3 Hackathon — [Lucidify](https://github.com/Seung-zedd/lucidify):** Built a multimodal lucid-dreaming
  interface (Gemini 2.5 Flash, Veo 3.1, Imagen 4.0) end-to-end within the hackathon window — SvelteKit + GCP serverless.
- **AI 포텐데이 x Naver Cloud Hackathon:** Led backend + AI/STT integration for EchoBloom, shipping a full
  plan-to-release cycle in 20 days.

---
📫 **How to reach me:**
- **LinkedIn:** [![My LinkedIn](https://img.shields.io/badge/LinkedIn%20Profile-SeungJe-blue?logo=data:image/svg%2bxml;base64,PHN2ZyByb2xlPSJpbWciIGZpbGw9IiNmZmZmZmYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+TGlua2VkSW48L3RpdGxlPjxwYXRoIGQ9Ik0yMC40NDcgMjAuNDUyaC0zLjU1NHYtNS41NjljMC0xLjMyOC0uMDI3LTMuMDM3LTEuODUyLTMuMDM3LTEuODUzIDAtMi4xMzYgMS40NDUtMi4xMzYgMi45Mzl2NS42NjdIOS4zNTFWOWgzLjQxNHYxLjU2MWguMDQ2Yy40NzctLjkgMS42MzctMS44NSAzLjM3LTEuODUgMy42MDEgMCA0LjI2NyAyLjM3IDQuMjY3IDUuNDU1djYuMjg2ek01LjMzNyA3LjQzM2MtMS4xNDQgMC0yLjA2My0uOTI2LTIuMDYzLTIuMDY1IDAtMS4xMzguOTItMi4wNjMgMi4wNjMtMi4wNjMgMS4xNCAwIDIuMDY0LjkyNSAyLjA2NCAyLjA2MyAwIDEuMTM5LS45MjUgMi4wNjUtMi4wNjQgMi4wNjV6bTEuNzgyIDEzLjAxOUgzLjU1NVY5aDMuNTY0djExLjQ1MnpNMjIuMjI1IDBIMS43NzFDLjc5MiAwIDAgLjc3NCAwIDEuNzI5djIwLjU0MkMwIDIzLjIyNy43OTIgMjQgMS43NzEgMjRoMjAuNDUxQzIzLjIgMjQgMjQgMjMuMjI3IDI0IDIyLjI3MVYxLjcyOUMyNCAuNzc0IDIzLjIgMCAyMi4yMjIgMGguMDAzeiIvPjwvc3ZnPgo=)](https://www.linkedin.com/in/seung-zedd/)


