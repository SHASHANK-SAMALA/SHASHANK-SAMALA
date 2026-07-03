### Hi, I'm Shashank 👋
**AI/Backend Engineer — building agentic systems with LangGraph & MCP, shipping backend services at EPAM Systems**

I build multi-agent systems that do more than wrap an LLM call — routing logic, memory, evaluation loops, and human approval gates before anything touches real state. By day I write FastAPI microservices and CI/CD pipelines at EPAM.

📫 [LinkedIn](https://linkedin.com/in/shashank-samala) · [Portfolio](https://shashank77-portfolio.netlify.app) · shashanksamala77@gmail.com

---

#### 🧠 What I've built

**AI E-Commerce Operations Brain** — [repo link](https://github.com/SHASHANK-SAMALA/E-commerce-Operations-Brain)
7-agent LangGraph system — coordinator, 4 parallel domain agents (sales, inventory, marketing, support), memory, and reflection — that diagnoses revenue anomalies in under 15 seconds.
- Two-stage router: deterministic rules resolve 95% of queries at zero LLM cost, GPT-4o handles the rest
- 16 regex-based prompt-injection filters, plus human-in-the-loop approval before any state-changing action runs
- Three-layer memory (Redis, pgvector+Postgres, Mem0), OpenTelemetry + LangSmith tracing, DeepEval in CI

`LangGraph` `Azure OpenAI` `MCP` `pgvector` `Redis` `React`

**Multi-Agent AI Orchestrator** — [repo link](https://github.com/SHASHANK-SAMALA/langraph_mcp)
Supervisor-agent system — 3 specialists (CI/CD, Productivity, Market) talking to 5 MCP tool servers (GitHub, Gmail, Calendar, Stock, Tavily).
- Self-healing CI/CD agent: reads a failed GitHub Actions log → finds a fix via Tavily → writes a patch → tests it in a sandbox → opens a PR for human approval
- Evaluator node scores every response 1–5 on accuracy/completeness/actionability, auto-retries up to 2x below threshold

`LangGraph` `MCP` `Gemini 1.5` `WebSockets` `FastAPI`

---

#### 🛠️ Core stack
`Python` `FastAPI` `LangGraph` `MCP` `PostgreSQL/pgvector` `Redis` `Docker` `AWS` `GitHub Actions`
