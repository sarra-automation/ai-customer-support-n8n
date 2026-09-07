# AI-Powered Customer Support & Automation Pipeline

An automated, production-ready customer support pipeline built using *n8n*, *Docker*, *Google Gemini API*, and *Google Sheets*, featuring secure environment variables and automated error monitoring via Gmail.

## 🚀 Overview

This workflow automates the incoming customer support process:
1. *Trigger:* Captures customer inquiries via web forms/webhooks.
2. *AI Processing:* Uses Google Gemini API to analyze intent, extract critical parameters, and formulate tailored responses.
3. *Data Logging:* Automatically updates Google Sheets with structured records of all inquiries and actions.
4. *Resilience & Monitoring:* Includes an integrated Error Handling workflow that captures execution failures and triggers instant email alerts via Gmail.

## 🛠️ Tech Stack

* *Orchestration:* n8n (Self-hosted via Docker Desktop / WSL2)
* *AI Model:* Google Gemini API
* *Database & Storage:* Google Sheets
* *Notifications:* Gmail Node
* *Environment:* Managed securely using Docker .env files

## 🔒 Security & Best Practices

* *Zero Hardcoded Secrets:* Sensitive credentials and API keys are strictly referenced via environment variables ($env.GEMINI_API_KEY).
* *Error Resilience:* Features dedicated error triggers to log failure contexts without disrupting primary pipelines.

## 📦 How to Use

1. Download the workflow.json file from this repository.
2. Open your n8n instance and click *Import from File*.
3. Configure your credentials for Google Gemini API, Google Sheets, and Gmail inside n8n.
4. Activate the workflow!
