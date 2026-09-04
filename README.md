<div align="center">

# 李宗宽 / Air

**AI Agent & LLM Application Engineer · Master's Candidate in Communication Engineering**

Building controllable, recoverable, and evaluable AI Agent systems.  
Focused on **Agent Runtime / Harness, RAG evaluation, Context Engineering, and reliable backend systems**.

<p>
  <img src="https://img.shields.io/badge/Open%20to-2027%20Graduate%20Roles-4A78D0" alt="Open to 2027 Graduate Roles" />
  <a href="mailto:1113476369@qq.com"><img src="https://img.shields.io/badge/Email-1113476369%40qq.com-2E8B57" alt="Email" /></a>
</p>

</div>

## Engineering Highlights

- **Agent Runtime / Harness** — bounded Agent Loop, versioned Tool Contracts, persist-before-execute, experiment governance, crash reconciliation, cancellation, and deterministic result validation.
- **RAG Evaluation** — frozen TechQA benchmark with **28,481 documents / 610 answerable queries**; Dense Top-100 + rerank improved held-out Recall@5 from **64.4% → 72.5% (+8.1pp)** and MRR@10 from **0.519 → 0.561**.
- **Backend Engineering** — Python / FastAPI / PostgreSQL, async workflows, state machines, database migrations, automated tests, CI, and reproducible local environments.

## Featured Projects

### 1. [LabPilot — AI Agent Runtime / Harness](https://github.com/Air000000/LabPilot)

A controllable, recoverable, and verifiable runtime for machine-learning experiments. It separates Agent decisions, human approval, physical execution, recovery, and deterministic result validation instead of letting an LLM directly control long-running training jobs.

**Engineering evidence:** fault-injection validation showed that a Coordinator restart could reconcile the original training Attempt **without a second physical launch**, with explicit cancellation paths for running and pre-launch work.

`Python` `FastAPI` `PostgreSQL` `asyncio` `Agent Runtime` `Context Engineering` `Tool Calling` `SSE`

---

### 2. [Enterprise Support AI Copilot — RAG + Controlled Ticket Agent](https://github.com/Air000000/Enterprise-Support-AI-Copilot-API)

An enterprise IT support backend combining document lifecycle management, RAG, controlled ticket creation, Human-in-the-loop approval, AgentOps tracing, and an offline evaluation pipeline.

**Held-out DEV:** Dense Top-100 + `qwen3-rerank` improved Recall@5 from **64.4% → 72.5% (+8.1pp)** and MRR@10 from **0.519 → 0.561** on a frozen TechQA benchmark.

`Python` `FastAPI` `SQLAlchemy` `ChromaDB` `RAG` `Rerank` `AgentOps` `Pytest`

---

### 3. [TimePrism — Local-first Desktop Productivity App](https://github.com/Air000000/timeprism)

A Windows-first local desktop app for understanding computer usage, work-rest rhythm, reminders, and focus signals. It captures foreground-app activity, applies privacy processing and local classification rules, stores data in SQLite, and provides review workflows and desktop-companion surfaces.

`Tauri` `Vue 3` `TypeScript` `Rust` `SQLite` `Local-first`

---

### 4. [CausalLift — BenchFlow / SkillsBench Agent Skill Evaluation](https://github.com/Air000000/causallift)

A leakage-controlled Agent Skill optimization and evaluation pipeline designed to distinguish reusable Skill improvements from public-task overfitting.

**Evaluation design:** frozen **60 / 17 / 10 Dev–Holdout–Final-Blind split**, explicit `no_skill` vs `with_skill` paired runs, execution provenance, regression gates, and generalization checks.

`Python` `Agent Skills` `BenchFlow` `SkillsBench` `Agent Evaluation` `Docker`

## Other Projects

- **[Codex History Restorer](https://github.com/Air000000/codex-history-restorer)** — local Windows tool for recovering Codex Desktop conversations that still exist on disk but no longer appear in the application.
- **[Bilibili Content](https://github.com/Air000000/bilibili-content)** — reusable CLI tool and AI Skill for subtitle extraction, validation, transcription, and structured downstream processing.

## Tech Stack

- **Agent / LLM:** Context Engineering · Tool / Function Calling · Human-in-the-loop · RAG · Retrieval / Rerank · Agent Evaluation
- **Backend:** Python · FastAPI · asyncio · SQLAlchemy · PostgreSQL · SQLite
- **Engineering:** Pytest · Alembic · GitHub Actions · Docker Compose · Git · Linux / Shell · Ruff · mypy
- **Product / Desktop:** TypeScript · Vue 3 · Rust · Tauri
- **Research:** PyTorch · causal discovery · causal representation learning · generative models · counterfactual generation

## Research

Master's candidate in Communication Engineering, researching causal structure learning for diffusion-based generative models, including causal discovery, causal representation learning, and counterfactual image generation.

First-author manuscript submitted to *Neurocomputing*.
