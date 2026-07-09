# 🤖 InsightGPT – AI Business Analyst

An AI-powered Business Intelligence Assistant built using **Flowise**, **Google Gemini**, **PostgreSQL MCP**, and **Supabase**. The application converts natural language questions into SQL queries and retrieves business insights from a PostgreSQL database.

---

## 🚀 Project Overview

InsightGPT allows business users to ask questions in plain English without writing SQL.

Instead of manually querying a database, users can ask questions like:

- How many customers are there?
- List all tables.
- Show the top 5 customers.
- Count customers by market.

The AI agent understands the question, generates the appropriate SQL query, executes it safely using PostgreSQL MCP, and returns the results in a readable table.

---

## ✨ Features

- 🤖 Ask questions in plain English
- 🧠 Google Gemini converts natural language into SQL
- 🗄️ Read-only PostgreSQL access using MCP
- 🔒 Secure database interaction
- 📊 Results displayed in Markdown tables
- ⚡ Built using Flowise Tool Agent
- 📈 Business-friendly insights without writing SQL

- ## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Flowise | AI workflow orchestration |
| Google Gemini 2.5 Flash | Large Language Model (LLM) |
| PostgreSQL MCP | Secure database tool execution |
| Supabase | PostgreSQL database hosting |
| PostgreSQL | Relational database |
| Prompt Engineering | SQL generation and business insights |
| GitHub | Version control and project hosting |

## 🏗️ Architecture

```text
                +----------------------+
                |       User           |
                +----------+-----------+
                           |
                           | Natural Language Question
                           |
                           ▼
                +----------------------+
                |  Flowise Tool Agent  |
                +----------+-----------+
                           |
              +------------+------------+
              |                         |
              ▼                         ▼
     +----------------+        +--------------------+
     | Google Gemini  |        | PostgreSQL MCP     |
     | 2.5 Flash LLM  |        | Read-only Database |
     +----------------+        +---------+----------+
                                         |
                                         ▼
                              +----------------------+
                              | Supabase PostgreSQL  |
                              +----------------------+
                                         |
                                         ▼
                              SQL Results & Insights
```
