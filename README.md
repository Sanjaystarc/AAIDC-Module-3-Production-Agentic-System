# AAIDC Module 3 – Production Agentic System

This project implements a **production-ready autonomous task planner** using an **agentic control loop**. It is developed as part of **Module 3** of the *Agentic AI Developer Certification (AAIDC)*.

The system demonstrates how an AI agent can safely plan, execute, evaluate, and adapt tasks while enforcing strict termination and safety constraints.

---

## 🚀 Features

- Agentic **Plan → Execute → Evaluate → Replan** workflow
- Modular architecture with clear separation of responsibilities
- Safety-bounded autonomy with retry and termination limits
- LLM-powered task execution (Groq-based)
- Streamlit UI for interactive testing
- Environment-based configuration management

---

## 📂 Project Structure

```
AAIDC-Module-3-Production-Agentic-System/
│
├── main.py # Entry point – orchestrates the agentic loop
├── planner.py # Task planning logic
├── executor.py # Task execution strategies
├── executor_llm.py # LLM-powered execution using Groq
├── evaluator.py # Output evaluation and decision logic
├── state.py # Execution state management
├── tools.py # Utility tools for generation and validation
├── ui.py # Streamlit-based UI
├── config.py # Central configuration
├── env.example # Example environment variables
├── requirements.txt # Python dependencies
├── README.md # Project documentation
└── LICENSE # License information
```

---

## 🧠 How It Works

1. A user provides a **high-level goal**
2. The **Planner Agent** decomposes it into executable tasks
3. The **Executor Agent** performs each task
4. The **Evaluator Agent** validates task outputs
5. The **State Manager** tracks progress and retries
6. The system safely:
   - Continues
   - Retries
   - Replans
   - Terminates

This ensures reliable and controlled autonomous execution.

---

## 🛠️ Setup Instructions

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Sanjaystarc/AAIDC-Module-3-Production-Agentic-System.git
cd AAIDC-Module-3-Production-Agentic-System


