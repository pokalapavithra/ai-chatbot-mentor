🧑‍🏫 AI Chatbot Mentor
A Controlled, Module-Based AI Learning Assistant

AI Chatbot Mentor is an intelligent mentoring application designed to deliver precise and focused learning support by restricting AI responses to user-selected technical domains. The system avoids generic AI behavior and ensures that learning remains structured, relevant, and reliable.

This project demonstrates how LLMs can be safely and effectively used in education through strict prompt control and domain enforcement.

🔍 Motivation

Most AI chatbots attempt to answer every question, often resulting in:

Hallucinated responses

Topic drift

Inconsistent explanations

This project solves that problem by enforcing domain boundaries, allowing the AI to function as a true mentor rather than a general-purpose chatbot.

⚙️ How the System Works

User selects a learning module

Questions are validated against the selected domain

LangChain enforces domain-specific prompt rules

LLM generates controlled responses

Chat history is stored and can be exported

Out-of-scope questions are explicitly rejected.

🧠 Core Capabilities

Domain-Constrained Responses
Ensures the AI answers only within the selected module

Hallucination Prevention
Rejects unrelated or off-topic questions

Session-Level Memory
Maintains conversational flow within a mentoring session

Downloadable Chat Logs
Enables offline review and revision

Simple & Clean UI
Built using Streamlit for ease of use

📚 Supported Domains

Python

SQL

Power BI

Exploratory Data Analysis (EDA)

Machine Learning

Deep Learning

Generative AI

Agentic AI

🏗️ Architecture Overview
``` bash d
User
 ↓
Streamlit Interface
 ↓
Module Selection
 ↓
LangChain Prompt Controller
 ↓
Large Language Model
 ↓
Mentor Response
 ↓
Chat History & Export
```
🛠️ Technology Stack
``` bash
Frontend:             Streamlit

Prompt Orchestration: LangChain

Language Model:       Hugging Face LLMs

Backend Language:     Python

Secrets Management: python-dotenv
```
``` bash
📁 Repository Structure
ai-chatbot-mentor/
├── chat/
│   ├── files/
│   │   ├── main.py
│   │   ├── req.txt
│   │   └── .env (ignored)
│   └── etc/
├── .gitignore
└── README.md
```
🚀 Getting Started
Clone the Repository
``` bash
git clone https://github.com/madhava-raju/ai-chatbot-mentor.git
cd ai-chatbot-mentor
```
Install Dependencies
``` bash
pip install -r chat/files/req.txt
```
Configure Environment
Create a .env file inside chat/files/:
``` bash
HUGGINGFACEHUB_API_TOKEN=your_api_key
```
Run the App
``` bash
streamlit run chat/files/main.py
```
🌐 Deployment

This application can be deployed on Streamlit Community Cloud by configuring repository secrets for the Hugging Face API key.

🎯 Learning Outcomes

Designing safe and controlled AI systems

Domain-restricted prompt engineering

LangChain-based LLM orchestration

Secure handling of API keys

Building real-world educational AI tools

📌 Final Notes

AI Chatbot Mentor showcases how LLMs can be used responsibly for learning by prioritizing accuracy over breadth. The project serves as a strong foundation for advanced educational AI systems.
