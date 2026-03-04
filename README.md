# 🤖 NotebookLM · Customer Feedback Intelligence System

> An AI-powered product intelligence system to analyze customer feedback, detect bottlenecks, and prioritize initiatives using the RICE framework.

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Powered by NotebookLM](https://img.shields.io/badge/Powered%20by-NotebookLM-blue)
![Framework: RICE](https://img.shields.io/badge/Framework-RICE-green)
![PM Ready](https://img.shields.io/badge/PM-Ready-orange)

---

## 🎯 What is this project?

This repository is an **open, replicable methodology** that enables product teams to:

1. **Centralize** all customer feedback into structured PDFs
2. **Load them into NotebookLM** as an AI-queryable knowledge base
3. **Use specialized prompts** to detect patterns, bottlenecks, and opportunities
4. **Prioritize** the resulting initiatives using the **RICE framework**
5. **Make product decisions** based on evidence, not intuition

---

## 🧠 Why NotebookLM?

NotebookLM (by Google) is different from other AI assistants because:

- ✅ **Only answers from your documents** — no hallucinations from the internet
- ✅ **Cites the exact source** of every insight — every claim is verifiable
- ✅ **Connects patterns** across multiple PDFs simultaneously
- ✅ **Accepts up to 50 sources** per notebook (500,000 words per document)
- ✅ **Free** in its basic version, with a Plus option for teams

---

## 🚀 Quick Start

### Step 1 — Prepare your feedback PDFs
Follow the conventions in [`/pdf-structure/feedback-pdf-template.md`](./pdf-structure/feedback-pdf-template.md)

### Step 2 — Set up your Notebook in NotebookLM
Read the guide in [`/notebook-setup/notebook-configuration.md`](./notebook-setup/notebook-configuration.md)

### Step 3 — Load the Master Prompt
Copy the prompt from [`/prompts/master-prompt.md`](./prompts/master-prompt.md) into the notebook instructions section

### Step 4 — Run the analysis prompts
Use the specialized prompts in `/prompts/` depending on what you need to investigate

### Step 5 — Prioritize with RICE
Bring your findings into the matrix at [`/rice-framework/rice-matrix-template.md`](./rice-framework/rice-matrix-template.md)

---

## 📂 Repository Structure

| Folder | Description |
|---|---|
| `/prompts` | Master prompt and specialized prompts for NotebookLM |
| `/rice-framework` | Guides, templates, and examples for the RICE framework |
| `/pdf-structure` | How to structure and name feedback PDFs |
| `/notebook-setup` | Optimal notebook configuration in NotebookLM |
| `/examples` | Sample outputs and completed RICE matrices |

---

## 👥 Who is this for?

- 🛠️ **Product Managers** handling large volumes of customer feedback
- 📊 **Data Scientists** looking to structure qualitative insights
- 🤖 **AI/ML Teams** integrating LLMs into PM workflows
- 🏢 **Product Leaders** who need data-driven prioritization

---

## 🤝 Contributing

Have improvements to the prompts or framework? Read [`CONTRIBUTING.md`](./CONTRIBUTING.md).

---

## 📄 License

MIT License — use it, adapt it, and share it freely.
