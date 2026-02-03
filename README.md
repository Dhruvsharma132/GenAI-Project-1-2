# GenAI Project 1–2 — Agentic AI & Conversational Systems

> Solutions for Soulpage’s Generative AI assignments demonstrating multi-agent orchestration and conversational AI with memory & tools.

This repository presents two hands-on implementations highlighting advanced Generative AI system design using **LangGraph-style agent workflows** and **context-aware conversational agents**.

# 🧠 Soulpage GenAI Assignment — Dhruv Sharma

This repository contains solutions for the **Soulpage GenAI Assignment**, focused on designing **agentic AI systems** using **LangGraph and LangChain-style architectures**.

The assignment is implemented through two tasks:

- **Task 1:** Multi-Agent System using LangGraph  
- **Task 2:** Conversational Knowledge Bot with Memory and Tools  

Both tasks are provided as **fully annotated Jupyter notebooks** to ensure reproducibility, clarity, and ease of evaluation.

---

## 📁 Repository Structure

```
Soulpage-genai-assignment-dhruvsharma/
│
├── Task1_Multi_Agent_LangGraph_Submission.ipynb
├── Task2_Conversational_Knowledge_Bot_Submission.ipynb
├── README.md
└── requirements.txt (optional)
```

---

## ✅ Task 1: Multi-Agent System using LangGraph

### 📌 Objective
Design an **agentic AI system** with two or more collaborating agents that perform a **multi-step task**, while maintaining shared context and explicit orchestration.

This task evaluates:
- Understanding of agent workflows
- Tool or data abstraction
- LangGraph-based orchestration
- Shared state (memory) between agents

---

### 🧩 System Overview

The system is implemented as a **Company Intelligence Agentic System** with the following components:

#### 🔹 Data Collector Agent
- Acts as **Agent 1**
- Gathers structured company-related information (simulated data)
- Writes results to shared state

#### 🔹 Analyst Agent
- Acts as **Agent 2**
- Consumes collected data
- Generates:
  - Executive summary  
  - Key opportunities  
  - Potential risks  

#### 🔹 LangGraph Orchestrator
- Explicitly controls execution order
- Manages shared state between agents
- Ensures deterministic, multi-step workflow execution

---

### 🧠 Key Design Decisions
- **LangGraph** is used instead of simple chains to explicitly model agent workflows.
- **Shared state (`AgentState`)** acts as memory between agents.
- **Mocked data and reasoning outputs** are used to:
  - Avoid external API dependencies
  - Ensure reproducibility for evaluators
  - Focus evaluation on agent design and orchestration

---

### ▶ How to Run Task 1

```bash
jupyter notebook Task1_Multi_Agent_LangGraph_Submission.ipynb
```

---

### 📄 Sample Output

```
===== COMPANY INTELLIGENCE REPORT =====

Executive Summary:
OpenAI is a major player in the AI industry with strong technological influence.

Key Opportunities:
- Expansion into enterprise AI solutions
- Research partnerships
- Developer ecosystem growth

Potential Risks:
- Regulatory and compliance pressure
- High infrastructure costs
- Competitive market landscape
```

---

## ✅ Task 2: Conversational Knowledge Bot (LangChain + Tools + Memory)

### 📌 Objective
Build a **conversational knowledge bot** capable of:
- Remembering previous conversation turns
- Searching external data (simulated knowledge base)
- Answering contextual, multi-turn queries

This task evaluates:
- Conversational memory handling
- Tool integration
- Context-aware response generation

---

### 🧩 System Overview

The conversational bot consists of:

#### 🔹 Conversation Memory
- A buffer that stores user and bot messages
- Enables follow-up questions using prior context
- Conceptually equivalent to LangChain’s `ConversationBufferMemory`

#### 🔹 Knowledge Tool
- A static knowledge base simulating Wikipedia or search APIs
- Queried dynamically based on user input

#### 🔹 Conversational Agent
- Combines memory and tool usage
- Tracks conversational context (e.g., previously mentioned entities)
- Produces contextual responses across multiple turns

---

### ▶ How to Run Task 2

```bash
jupyter notebook Task2_Conversational_Knowledge_Bot_Submission.ipynb
```

---

### 💬 Sample Interaction

```
You: Who is the CEO of OpenAI?
Bot: Sam Altman

You: Where did he study?
Bot: He studied at Stanford University but dropped out.
```

---

## 🧠 Key Concepts Demonstrated

- Agentic AI system design
- Multi-agent collaboration
- LangGraph-based orchestration
- Memory and state management
- Tool-based knowledge retrieval
- Context-aware conversational flow
- Reproducible, evaluator-friendly notebooks

---

## 🚀 Why This Matters

This project showcases skills that are directly applicable to **real-world AI and ML engineering roles**, including:

✔ Designing agentic AI systems with clear modular structure  
✔ Building memory-augmented conversational applications  
✔ Deploying context-aware components for human-AI interaction  
✔ Reproducible, evaluator-friendly notebook implementations

Whether for internal tooling, digital assistants, or next-generation AI workflows, these patterns reflect **industry-relevant generative and agentic designs**.

---

## ▶️ How to Run

1. Open the repository in Jupyter Notebook
2. Run **Task1_Multi_Agent_LangGraph_Submission.ipynb**
3. Run **Task2_Conversational_Knowledge_Bot_Submission.ipynb**

---

## 📌 Skills & Technologies
**Key Skills Demonstrated**
- Agent-oriented AI design
- Generative AI workflows
- Context maintenance and conversational memory
- System architecture thinking for LLM-style agents

**Tools / Libraries (conceptual)**
- LangGraph-style orchestration
- Notebook-based deliverables

---

## 📈 Future Enhancements

You could expand this project to:
- Integrate real LLM APIs (OpenAI, LLaMA, Claude)
- Add external knowledge sources (wiki APIs, vector search)
- Containerized deployment (Docker, FastAPI)
- UI interface for conversational bot

---

## 🏁 Final Notes

- Both tasks strictly follow the assignment requirements.
- No external APIs or API keys are required.
- The solutions prioritize **clarity, modularity, and reproducibility**.
- The architecture is **model-agnostic** and can be extended to real LLMs or APIs if needed.

---

## 📌 Author

**Dhruv Sharma** — MSc in Data Science | Applied AI & ML  
*Portfolio:* https://github.com/Dhruvsharma132  
*LinkedIn:* https://www.linkedin.com/in/dhruv-sharma-4791b723a/
