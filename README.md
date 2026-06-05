# 2026 PRISM-AI InnoCORE Workshop

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> **PRISM-AI InnoCORE Research Center, KAIST**  
> Dept. of Mechanical Engineering · June 4–5, 2026  
> 🗣 Sessions conducted in **Korean** · AI simultaneous interpretation into **English** will be provided

---

## Wi-Fi

| | |
|-|-|
| **Network** | `welcome_kaist` |
| **ID** | `kaist_innocore` |
| **Password** | `prismai1!` |

> If you have trouble connecting, please use your personal mobile data or hotspot.

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
| 15:00 – 15:30 | **InnoCORE Program Talk & Q&A** · [Prof. Seunghwa Ryu](https://sites.google.com/site/seunghwalab/home?authuser=0) (Director) | KAIST 기계공학동 대회의실 |
| 15:30 – 16:00 | **Program Introduction** · Staff | KAIST 기계공학동 대회의실 |
| 16:00 – 16:30 | Coffee Break | 중앙회의동 해동정보홀 |
| 16:30 – 18:00 | **Poster Session** — postdoc research presentations | 중앙회의동 해동정보홀 |
| 18:00 – | Dinner & Career Consulting | [만년동 일정](https://naver.me/5S94wfmr) |
| | **Career Consulting Mentors:** | |
| | &nbsp;&nbsp;· [Prof. Jeong Whan Yoon](https://canesm.kaist.ac.kr/) (KAIST) | |
| | &nbsp;&nbsp;· [Prof. Ikjin Lee](http://idol.kaist.ac.kr/) (KAIST) | |
| | &nbsp;&nbsp;· [Prof. Seungchul Lee](https://iailab.kaist.ac.kr/) (KAIST) | |
| | &nbsp;&nbsp;· [Prof. Namwoo Kang](https://www.smartdesignlab.org/) (KAIST) | |
| | &nbsp;&nbsp;· [Prof. KyungTae Lim](https://sites.google.com/view/aailab) (KAIST) | |
| | &nbsp;&nbsp;· [Prof. Seunghwa Ryu](https://sites.google.com/site/seunghwalab/home?authuser=0) (KAIST) | |
| | &nbsp;&nbsp;· Dr. Jaemin Lee (Senior Researcher, Agency for Defense Development) | |

### Day 2 — Friday, June 5

| Time | Program | Venue |
|------|---------|-------|
| 10:00 – 12:00 | **LLM Lecture (1)** | 중앙회의동 해동정보홀 |
| | &nbsp;&nbsp;· Colab environment setup + LangChain tutorial · Jonmin Park, Ph.D. (PRISM-AI) | |
| | &nbsp;&nbsp;· RAG tutorial · Junhyeong Lee, Ph.D. (PRISM-AI) | |
| 12:00 – 13:00 | Lunch | KAIST 카이마루 |
| 13:00 – 15:00 | **LLM Lecture (2)** | 중앙회의동 해동정보홀 |
| | &nbsp;&nbsp;· Multi-agent system development · Junhyeong Lee, Ph.D. (PRISM-AI) | |
| | &nbsp;&nbsp;· Vibe coding tools · Hyeok Jae Chae, Wonjong Jeong (PRISM-AI) · [Materials](vibecoding_codex_example_WonjongJeong.pdf) | |

> ※ Schedule is subject to minor changes.

---

## Venues

| Location | Used for |
|----------|----------|
| KAIST 기계공학동 대회의실 | Day 1 — Invited lecture, InnoCORE Q&A |
| KAIST 중앙회의동 해동정보홀 | Day 1 — Coffee break, Poster session · Day 2 — LLM lectures |
| KAIST 카이마루 | Day 2 — Lunch |
| [만년동 일정](https://naver.me/5S94wfmr) | Day 1 — Dinner & career consulting |

---

## Lecture Materials

All lecture materials (slides, references, etc.) are available at the link below:

👉 [Google Drive — Lecture Materials](https://drive.google.com/drive/folders/1sstAhb5Ila3hLeQYLJpQXY6FXs84cDY3?usp=drive_link)

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

### Opening Notebooks via Google Drive (Recommended)

**Step 1 — Download the notebook**
1. Click the notebook link in the table above
2. On the GitHub preview page, click the **Download raw file** button (↓ icon, top-right)
3. Save the `.ipynb` file to your computer

**Step 2 — Upload to Google Drive**
1. Go to [drive.google.com](https://drive.google.com)
2. Create a folder (e.g. `PRISM-AI Workshop`) and open it
3. Drag and drop the `.ipynb` file into the folder

**Step 3 — Open in Colab**
1. Double-click the `.ipynb` file in Drive
2. It should open automatically in Google Colab

> ⚠️ **If the file doesn't open in Colab** (opens as plain text instead):
> Colab may not be installed as a connected app. Fix it once:
> 1. In Google Drive, click **+ New → More → Connect more apps**
> 2. Search for **"Colaboratory"** and click **Install**
> 3. Click **OK** → now double-clicking any `.ipynb` will open Colab automatically

---

### Dependencies

```
langchain langchain-openai langchain-community
faiss-cpu pypdf tiktoken beautifulsoup4
langgraph
autogen-agentchat autogen-ext[openai] nest_asyncio
```


