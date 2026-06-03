# 2026 PRISM-AI InnoCORE Workshop
### LLM Tutorial Materials

> **PRISM-AI InnoCORE Research Center, KAIST**  
> Dept. of Mechanical Engineering · June 4–5, 2026

---

## Overview

This repository contains hands-on tutorial notebooks for the **LLM lecture session** of the 2026 PRISM-AI InnoCORE Workshop. The workshop brings together postdoctoral researchers across the PRISM-AI consortium to share research progress, explore collaboration opportunities, and build practical AI skills.

**Workshop goals:**
- Share PRISM-AI research directions and InnoCORE program updates
- Provide career development insights from senior researchers
- Enable postdocs to integrate LLM technologies into their own research domains
- Strengthen interdisciplinary collaboration through poster sessions and networking

---

## Program Schedule

### Day 1 — Thursday, June 4

| Time | Program | Venue |
|------|---------|-------|
| 13:30 – 14:00 | Registration & Check-in | KAIST 기계공학동 대회의실 |
| 14:00 – 15:00 | **Invited Lecture** — *"Postdoc Career Development"* · Prof. Yoon-Young Kim | KAIST 기계공학동 대회의실 |
| 15:00 – 16:00 | **InnoCORE Program Talk & Q&A** · Prof. Seunghwa Ryu (Director) | KAIST 기계공학동 대회의실 |
| 16:00 – 16:30 | Coffee Break | 중앙회의동 해동정보홀 |
| 16:30 – 18:00 | **Poster Session** — postdoc research presentations | 중앙회의동 해동정보홀 |
| 18:00 – | Dinner & Career Consulting | Nearby restaurant |

### Day 2 — Friday, June 5

| Time | Program | Venue |
|------|---------|-------|
| 10:00 – 12:00 | **LLM Lecture (1)** — *"Setting Up Environments for Multi-Agent Systems"* · Junhyeong Lee | 중앙회의동 해동정보홀 |
| 12:00 – 13:00 | Lunch | KAIST 카이마루 |
| 13:00 – 15:00 | **LLM Lecture (2)** — *"Applying Multi-Agent Systems to Your Research"* · Junhyeong Lee | 중앙회의동 해동정보홀 |

> ※ Schedule is subject to minor changes.

---

## Venues

| Location | Used for |
|----------|----------|
| KAIST 기계공학동 대회의실 | Day 1 — Invited lecture, InnoCORE Q&A |
| KAIST 중앙회의동 해동정보홀 | Day 1 — Coffee break, Poster session · Day 2 — LLM lectures |
| KAIST 카이마루 | Day 2 — Lunch |
| Nearby restaurant (TBD) | Day 1 — Dinner & career consulting |

---

## Tutorial Notebooks

All notebooks run on **Google Colab** — no local setup required. Replace `"YOUR API KEY"` with your OpenAI API key in the first cell.

| Notebook | Topics Covered |
|----------|---------------|
| [Tutorial 1 — LangChain Basics](PRISM-AI%20Tutorial_1.ipynb) | LLM chains, prompt engineering, memory, chatbot |
| [Tutorial 2 — RAG](PRISM-AI%20Tutorial_2.ipynb) | Document loading, text splitting, FAISS vector store, RAG chain, conversational RAG |
| [Tutorial 3 — Multi-agent Systems](PRISM-AI%20Tutorial_3.ipynb) | LangGraph (StateGraph, conditional edges, ReAct agent, Supervisor pattern), AutoGen (RoundRobin, SelectorGroupChat, tool-using agents) |

### Quick Start (Colab)

1. Open any notebook via the links above (or Google Colab → File → Open notebook → GitHub tab)
2. Set your API key:
   ```python
   import os
   os.environ['OPENAI_API_KEY'] = "sk-..."
   ```
3. Run all cells top to bottom

### Dependencies

```
langchain langchain-openai langchain-community
faiss-cpu pypdf tiktoken beautifulsoup4
langgraph
autogen-agentchat autogen-ext[openai] nest_asyncio
```

---

## Featured Research: IM-Chat

One highlight from the poster session — developed by the tutorial lecturer:

**"LLM-based Knowledge Transfer System for Injection Molding: Implementation and Performance Enhancement"**  
*Junhyeong Lee, Joon-Young Kim, Heekyu Kim, Inhyo Lee, Seunghwa Ryu*  
KAIST InnoCORE PRISM-AI Center

**IM-Chat** is a Supervisor-Worker multi-agent LLM framework for injection molding process decision support. It integrates RAG, tool-calling, and a diffusion-model-based process condition generator (CFGDM), enabling natural language-driven decision support for non-expert operators.

```
User Query
    │
    ▼
[Task Formatter + Translator]
    │
    ▼
[Classifier] ── Non-IM query ──▶ [ReAct Agent + Internet Search]
    │
    └── IM query ──▶ [Planner] ──▶ [Executor]
                          ↑              │
                     [Replanner] ◀─ [Supervisor] ──▶ [Reporter]
                                        Tools:
                                        ① Internet Search
                                        ② Troubleshooting Table
                                        ③ Manufacturing Manual
                                        ④ CFGDM (Diffusion Model)
```

---

## About PRISM-AI

**PRISM-AI** (*Platform for Real-world Innovation in Smart Manufacturing through AI*) is a Korean national research consortium funded under the InnoCORE initiative.

| | |
|-|-|
| **Director** | Prof. Seunghwa Ryu, KAIST Dept. of Mechanical Engineering |
| **Duration** | 2025 – 2029 (5 years, 2 phases) |
| **Budget** | 37.5 billion KRW total |
| **Postdocs** | 50/year (250 total), incl. 16 international fellows |
| **Partners** | 24 industry teams (Hyundai Motor, LG, Samsung Heavy Industries, …) · 14 government labs (KIMM, KITECH, KIMS, …) |
| **Global advisors** | MIT · UC Berkeley · DTU · UMD |

**5 Research Groups:**

| Group | Focus | Accuracy Target |
|-------|-------|-----------------|
| Design | Multi-physics simulation + AI inverse design | ≥ 95% |
| Materials | PIML/GNN property prediction + LLM recommendation | ≥ 95% |
| Manufacturing | LLM-controlled multi-agent process optimization | ≥ 95% |
| Operations (PHM) | Predictive maintenance + LLM anomaly explanation | ≥ 99% |
| AI Interface | Natural language platform for non-expert users | ≥ 90% |

---

## Contact

**Junhyeong Lee** — LLM Lecture  
KAIST InnoCORE PRISM-AI Center  
junhyeong8831@gmail.com
