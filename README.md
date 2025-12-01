# 5-Day Gen AI Intensive: AI Agents (Google x Kaggle)

![Banner](https://img.shields.io/badge/Gen_AI-Intensive_Course-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Tech](https://img.shields.io/badge/Tech-Vertex_AI_%7C_Gemini_%7C_LangGraph-blueviolet?style=for-the-badge)

## 📖 Overview

This repository hosts the complete codebase, notebooks, and learning materials from the **5-Day AI Agents Intensive**, a collaborative program by **Google** and **Kaggle** (Agent Workshop).

The program focused on the end-to-end lifecycle of building **Agentic AI systems** using Google's **Gemini 1.5** models. Unlike standard LLM scripting, this course emphasized autonomous agents capable of **reasoning, tool usage, interoperability (MCP), and production-grade deployment**.

## 📂 Repository Structure & Curriculum

The repository is structured to follow the daily intensive curriculum, progressing from foundational concepts to production deployment.

### [📂 Day-01-Introduction to Agents](./Day-01-Introduction%20to%20Agents)
**Theme:** The Anatomy of an Agent
*   **Focus:** Understanding the "Brain" (LLM), "Body" (Tools), and "Environment" of an AI agent.
*   **Key Implementations:**
    *   Setting up the `google-genai` SDK.
    *   Building a basic chat agent with reasoning capabilities.
    *   Transitioning from Zero-shot prompting to Few-shot agentic workflows.

### [📂 Day-02-Agent Tools & Interoperability with MCP](./Day-02-Agent%20Tools%20%26%20Interoperability%20with%20MCP)
**Theme:** Connecting Agents to the World
*   **Focus:** Enabling agents to take action using Function Calling and the **Model Context Protocol (MCP)**.
*   **Key Implementations:**
    *   **Function Calling:** Creating tools (calculators, search APIs) that Gemini can execute autonomously.
    *   **MCP (Model Context Protocol):** Implementing the standardized protocol for connecting AI assistants to data systems.
    *   Routing user queries between different tools based on intent.

### [📂 Day-03-Context Engineering: Sessions & Memory](./Day-03-Context%20Engineering:%20Sessions%20%26%20Memory)
**Theme:** Making Agents Smarter over Time
*   **Focus:** Managing state and context to allow for long-running, coherent conversations.
*   **Key Implementations:**
    *   **Session Management:** Handling user history across multiple turns.
    *   **Context Windows:** Strategies for managing token limits while retaining critical information.
    *   **Memory Stores:** Implementing short-term vs. long-term memory architectures.

### [📂 Day-04-Agent Quality](./Day-04-Agent%20Quality)
**Theme:** Trust, Safety, and Observability
*   **Focus:** How do we know the agent is doing the right thing?
*   **Key Implementations:**
    *   **Evals:** Running automated evaluation datasets to measure agent accuracy.
    *   **Tracing:** Visualizing the agent's "thought process" (Reasoning Traces) to debug logic errors.
    *   **Safety:** Implementing guardrails to prevent hallucinations or unsafe actions.

### [📂 Day-05-Prototype to Production](./Day-05-Prototype%20to%20Production)
**Theme:** Shipping the Agent
*   **Focus:** Moving from a Jupyter Notebook to a deployed application.
*   **Key Implementations:**
    *   **FastAPI / Flask Wrappers:** Serving the agent as a REST API.
    *   **Cloud Deployment:** Best practices for hosting agents on Google Cloud Platform (Vertex AI).
    *   **Capstone Concepts:** Architecture for scalable multi-agent systems.

---

## 🛠️ Technology Stack

*   **Models:** Google Gemini 1.5 Pro, Gemini 1.5 Flash
*   **Infrastructure:** Google Cloud Vertex AI
*   **Orchestration:** LangGraph / LangChain
*   **Protocols:** Model Context Protocol (MCP)
*   **Environment:** Python 3.10+, Jupyter Notebooks

## 🚀 How to Run the Code

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/AnandKumar56/Gen-AI-Intensive-Course-by-Kaggle-x-Google.git
    cd Gen-AI-Intensive-Course-by-Kaggle-x-Google
    ```

2.  **Install Dependencies:**
    It is recommended to use a virtual environment.
    ```bash
    pip install -q -U google-generativeai langchain langgraph notebook
    ```

3.  **API Key Configuration:**
    You must have a Google AI Studio API key.
    *   Create a `.env` file or export your key:
    ```bash
    export GOOGLE_API_KEY="your_api_key_here"
    ```

4.  **Explore the Notebooks:**
    Launch Jupyter and navigate to the folder of your choice:
    ```bash
    jupyter notebook
    ```

## 🏆 Acknowledgments

*   **Organizers:** Google Cloud & Kaggle (Gen AI Intensive Team).
*   **Instructors:** Google Developer Experts and ML Researchers.
*   **Collaborators:** Special thanks to the workshop cohort for the collaborative learning environment.

---
*Maintained by [AnandKumar56](https://github.com/AnandKumar56)*
