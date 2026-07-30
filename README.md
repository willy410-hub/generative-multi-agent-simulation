# 🤖 Generative Multi-Agent Dialogue Simulation

An end-to-end framework for orchestrating and simulating autonomous multi-agent conversations using **LangChain**, **Groq (Llama 3)**, and **Time-Weighted Memory Architecture**.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/willy410-hub/generative-multi-agent-simulation/blob/main/Multi_Agent_Simulation_Groq.ipynb)

---

## 📌 Key Features & Architecture

- **Generative Agents with Time-Weighted Memory:** Implements agent memory structures using FAISS vector retrieval weighted by recency, importance, and relevance.
- **Custom Dialogue Framework:** 
  - `DialogueAgent`: Manages individual agent system prompts, conversation history, and dynamic response generation using Groq's high-speed inference engine (`llama-3.1-8b-instant`).
  - `DialogueSimulator`: Orchestrates multi-agent conversation flow, turn-taking mechanisms, and message broadcasting across all active entities.
- **Enterprise-Grade Privacy:** Secure environment variable management via Colab Secrets (`userdata.get`) avoiding hardcoded API credentials.

---

## 🛠️ Tech Stack & Dependencies

- **Framework:** LangChain, LangChain-Community, LangChain-Experimental
- **LLM Engine:** Groq API (`llama-3.1-8b-instant`)
- **Vector Store & Retrieval:** FAISS, HuggingFace Embeddings (`all-MiniLM-L6-v2`)
- **Language:** Python 3.12

---

## 🚀 How to Run

1. Open the project directly in Google Colab using the **Open in Colab** badge above.
2. Add your Groq API Key to Colab **Secrets** (`GROQ_API_KEY`) and enable notebook access.
3. Run all cells sequentially to observe agent reactions, memory synthesis, and automated dialogue interaction.
