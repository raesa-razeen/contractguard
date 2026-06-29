# CONTRACTGUARD
## A Minimum Effective Human Oversight Framework for AI Agent Actions in Legal Documents

Built on LangGraph · Powered by Legal Fidelity Score · Tested on CUAD Benchmark

---

## The Problem
AI agents are autonomously modifying legal contracts.
Nobody is auditing what they actually did.
The EU AI Act (August 2026) requires demonstrable audit trails for high-risk AI systems.

---

## The Solution
CONTRACTGUARD is a 4-layer multi-agent system that:
- Detects every change an AI agent made to a contract
- Evaluates each change using the Legal Fidelity Score
- Scores risk deterministically using clause importance weights
- Identifies the minimum human review required
- Generates a defensible audit trail PDF

---

## Architecture

Agent 1 — The Watcher
Detects and logs every AI action on a contract.

Agent 2 — The Auditor
Evaluates each change using Legal Fidelity Score.
Classifies as FAITHFUL / MODIFIED / HALLUCINATED.

Agent 3 — The Risk Scorer
Scores each change deterministically.
Outputs minimum human review queue.

Agent 4 — The Reporter
Generates defensible audit trail PDF.

---

## Tech Stack
Python · LangGraph · LangChain · ChromaDB · Groq · Streamlit · FPDF2

---

## Dataset
Tested on CUAD — Contract Understanding Atticus Dataset
510 real legal contracts · 13,000+ expert annotations

---

## Connection to HALO
HALO evaluates what AI says about documents.
CONTRACTGUARD evaluates what AI does to documents.
Both powered by the Legal Fidelity Score from published ICCIC-2025 research.