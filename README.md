<div align="center">

# 李宗宽 / Air

**AI Agent 与大模型应用工程师 · 通信工程硕士在读**

致力于构建可控、可恢复、可评估的 AI Agent 系统。  
聚焦 **Agent 运行时与 Harness、RAG 评估、上下文工程和可靠的后端系统**。

<p>
  <img src="https://img.shields.io/badge/%E6%B1%82%E8%81%8C%E6%84%8F%E5%90%91-2027%20%E5%B1%8A%E6%A0%A1%E6%8B%9B-4A78D0" alt="求职意向：2027 届校招" />
  <a href="mailto:1113476369@qq.com"><img src="https://img.shields.io/badge/%E9%82%AE%E7%AE%B1-1113476369%40qq.com-2E8B57" alt="邮箱：1113476369@qq.com" /></a>
</p>

</div>

## 工程亮点

- **Agent 运行时与 Harness**：实现有边界的 Agent 循环、版本化工具契约、先持久化再执行、实验治理、故障后状态对账、取消机制和确定性结果校验。
- **RAG 评估**：基于固定的 TechQA 基准（**28,481 篇文档、610 条可回答查询**），Dense Top-100 + rerank 将留出集的 Recall@5 从 **64.4% 提升至 72.5%（+8.1 个百分点）**，MRR@10 从 **0.519 提升至 0.561**。
- **后端工程**：使用 Python、FastAPI 和 PostgreSQL，具备异步工作流、状态机、数据库迁移、自动化测试、CI 和可复现的本地环境实践经验。

## 代表项目

### 1. [LabPilot — AI Agent 运行时与 Harness](https://github.com/Air000000/LabPilot)

面向机器学习实验的可控、可恢复、可验证运行时。将 Agent 决策、人工审批、实际执行、故障恢复和确定性结果校验分开，避免让大模型直接控制长时间运行的训练任务。

**工程验证：**故障注入测试表明，Coordinator 重启后能够对账并恢复原训练 Attempt，**不会重复启动训练任务**；同时为运行中及启动前的任务提供明确的取消路径。

`Python` `FastAPI` `PostgreSQL` `asyncio` `Agent Runtime` `Context Engineering` `Tool Calling` `SSE`

---

### 2. [企业 IT 支持 AI Copilot — RAG 与受控工单 Agent](https://github.com/Air000000/Enterprise-Support-AI-Copilot-API)

企业 IT 支持后端，整合文档生命周期管理、RAG、受控工单创建、人工审批、AgentOps 链路追踪和离线评估流程。

**留出的 DEV 集结果：**在固定的 TechQA 基准上，Dense Top-100 + `qwen3-rerank` 将 Recall@5 从 **64.4% 提升至 72.5%（+8.1 个百分点）**，MRR@10 从 **0.519 提升至 0.561**。

`Python` `FastAPI` `SQLAlchemy` `ChromaDB` `RAG` `Rerank` `AgentOps` `Pytest`

---

### 3. [TimePrism — 本地优先的桌面效率应用](https://github.com/Air000000/timeprism)

面向 Windows 的本地桌面应用，帮助用户了解电脑使用情况、工作与休息节奏、提醒和专注状态。应用采集前台程序活动，在本地进行隐私处理和规则分类，将数据存入 SQLite，并提供回顾流程和桌面陪伴功能。

`Tauri` `Vue 3` `TypeScript` `Rust` `SQLite` `Local-first`

---

### 4. [CausalLift — BenchFlow / SkillsBench Agent Skill 评估](https://github.com/Air000000/causallift)

控制数据泄漏的 Agent Skill 优化与评估流程，用于区分可复用的 Skill 改进与针对公开任务的过拟合。

**评估设计：**固定的 **60 / 17 / 10 开发集、留出集与最终盲测集划分**，配对比较 `no_skill` 与 `with_skill` 的运行结果，并记录执行来源、设置回归门槛、检查泛化能力。

`Python` `Agent Skills` `BenchFlow` `SkillsBench` `Agent Evaluation` `Docker`

## 其他项目

- **[Codex History Restorer](https://github.com/Air000000/codex-history-restorer)**：Windows 本地工具，用于找回磁盘上仍有记录、但已不在 Codex Desktop 中显示的对话。
- **[Bilibili Content](https://github.com/Air000000/bilibili-content)**：可复用的命令行工具与 AI Skill，支持字幕提取、校验、转录及后续结构化处理。

## 技术栈

- **Agent / 大模型：**上下文工程 · 工具 / 函数调用 · 人工审批 · RAG · 检索 / 重排 · Agent 评估
- **后端：**Python · FastAPI · asyncio · SQLAlchemy · PostgreSQL · SQLite
- **工程实践：**Pytest · Alembic · GitHub Actions · Docker Compose · Git · Linux / Shell · Ruff · mypy
- **产品 / 桌面应用：**TypeScript · Vue 3 · Rust · Tauri
- **研究方向：**PyTorch · 因果发现 · 因果表征学习 · 生成模型 · 反事实生成

## 科研经历

通信工程硕士在读，研究方向为面向扩散生成模型的因果结构学习，包括因果发现、因果表征学习和反事实图像生成。

以第一作者身份向 *Neurocomputing* 投稿论文。
