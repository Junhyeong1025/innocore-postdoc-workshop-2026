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
| 14:00 – 15:00 | **Invited Lecture** — *"Postdoc Career Development"* · [Prof. Yoon Young Kim](https://www.yykimlab.net/) | KAIST 기계공학동 대회의실 |
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

### Getting an OpenAI API Key

1. Go to [https://platform.openai.com](https://platform.openai.com) and sign up / log in
2. Click your profile icon (top-right) → **API keys** → **Create new secret key**
3. Copy the key (starts with `sk-...`) — it won't be shown again
4. Add credits: **Settings → Billing → Add payment method** (minimum $5)

> ⚠️ Never share your API key or commit it to a public repository.

### Quick Start (Colab)

1. Open any notebook via the links above (or Google Colab → File → Open notebook → GitHub tab)
2. Set your API key in the first cell:
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


