# 🤖 AI Meeting Summarizer (n8n Workflow)

This repository contains an **n8n workflow** for automatically summarizing meeting transcripts using OpenAI and posting the results to Slack.

## 📂 Files
- `AI Meeting Summarizer.json` → The exported n8n workflow.

## 🚀 How it works
1. Workflow takes a **meeting transcript** as input.
2. Sends it to **OpenAI (GPT-3.5 Turbo)** via OpenRouter.
3. Returns a JSON response with:
   - Summary
   - Action items (with owner + due date if available)
   - Risks
4. Posts the formatted results to a **Slack channel**.

## 🔧 Setup
1. Import the `.json` workflow into your n8n instance.
2. Configure your **OpenRouter / OpenAI API key**.
3. Connect your **Slack account** (OAuth2).
4. Execute the workflow and get AI-powered meeting notes directly in Slack 🚀

## 📌 Example Input



---

## 📌 Example Output
**Summary**
- Conversion dropped  
- Suggest increasing ad budget  
- Risk of budget overruns  

**Action Items**
1. Allocate more budget to ads (Priya)  

**Risks**
1. Budget overruns  

---

👩‍💻 Created with [n8n](https://n8n.io), [OpenRouter](https://openrouter.ai), and Slack API
