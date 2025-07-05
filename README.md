<h1 align="center">🤖Code Review-Agent – Automated GitHub Code Reviewer with n8n + OpenAI + Telegram </h1>

<p align="center">
  <b>Automatically analyze pushed GitHub files with OpenAI and deliver results via Telegram</b>
</p>

---

## 📌 Workflow Overview

This <b>n8n workflow</b> performs the following tasks:

1. ⏰ Triggered when a new file is pushed to a GitHub repository
2. 📂 Extracts the file from the GitHub event
3. 🧠 Sends the file content to OpenAI API for analysis (e.g., scoring, feedback)
4. 📄 Formats the response as a score sheet or summary
5. 🚀 Delivers the result to a specified Telegram user or group

---
 <h2>⚙Setup Instructions</h2>
<h3>1️⃣ Import the Workflow into n8n</h3>
Go to your n8n editor UI

Click the top-right menu (⋮)

Choose <code>Import from file</code>

Upload <code>my-workflow.json</code> from this repository

<h3>2️⃣ Configure Required Credentials</h3>
Node	What You Need
GitHub	GitHub Personal Access Token (PAT)
OpenAI	OpenAI API Key
Telegram	Telegram Bot Token + Chat ID

🔐 <b>Warning:</b> Never hard-code real API keys in the JSON file. Always use n8n's Credential Manager.

<h3>3️⃣ Deploy and Activate</h3>
Save the workflow

Activate it (toggle top right)

Push a file to your connected GitHub repo and watch it work!

💡 Use Cases
Auto code reviews with AI

Content scoring (e.g., essays, assignments)

Feedback system for student submissions

CI-integrated report generator

🧪 Testing the Flow
To test:

Push a .js, .py, or .txt file to your GitHub repo

Wait a few seconds

You’ll receive a Telegram message with a score/feedback

