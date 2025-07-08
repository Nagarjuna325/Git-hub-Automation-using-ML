
# 🐞 BugHub: Data Pipeline & Knowledge Graph for GitHub & StackOverflow

**Project: BugHub - Team Collaboration & Knowledge Sharing Platform**

---


## 🧩 Project Overview

BugHub is a SaaS pilot project aiming to integrate and analyze data from **GitHub** and **StackOverflow** to:

- Build a data pipeline from both sources.
- Visualize defect distributions over the development life cycle.
- Construct a **Knowledge Graph** using `NetworkX`.
- Map StackOverflow questions to GitHub repositories based on tags and topics.
- Store and query data using a graph-based data model.

---

## 📌 Part 01 – Defect Analysis

📄 **`DRE_QM.ipynb`**

- Visualizes defect distribution over software lifecycle stages using data from:
  - `Release1.csv`
  - `Release2.csv`
- Uses `matplotlib` to create stacked bar charts for:
  - Requirements
  - Analysis
  - Design
  - Coding
  - Unit Testing
  - Integration Testing
  - System Testing
  - Field Errors

---

## 📌 Part 02 – GitHub & StackOverflow Integration

📄 **`Assignment_5_Part_2.ipynb`**, **`StackOverflow_Tags.ipynb`**

- Retrieves and processes:
  - GitHub repo metadata, issues, labels
  - StackOverflow tags, questions, answers
- Uses the **PyGitHub API** and StackExchange API
- Implements initial knowledge graph modeling with `networkx`

📜 **Helper Scripts:**

- `get_issues_details.py`: Gets issue metadata via GitHub API
- `get_repositories_details.py`: Retrieves repository-level info

---

## 📌 Part 03 – BugHub Knowledge Graph

📄 **`Assignment_5_Part_3 Sp.ipynb`**

- Combines GitHub and StackOverflow data into a **unified BugHub Knowledge Graph**
- Models relationships between:
  - Repositories ↔ Issues ↔ StackOverflow Tags
  - Contributors ↔ Repos
  - Tags ↔ Questions ↔ Answers
- Prepares schema for future ingestion into EdgeDB (EdgeQL/GraphQL)

---

## 🛠️ Setup Instructions

You can install the required packages manually:


pip install pandas numpy matplotlib networkx requests PyGithub
📈 Learning Outcomes
Construct real-world data pipelines

Integrate APIs (GitHub + StackOverflow)

Build and visualize knowledge graphs using networkx

Understand lifecycle defect distribution

Prepare for using graph databases like EdgeDB

🧾 Resources Used
GitHub REST API Docs

PyGitHub Library

StackExchange API

NetworkX Docs

EdgeDB Docs

👨‍🏫 Instructor
Atef Bader
Course: Software Project Management

