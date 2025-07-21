# 📩 Teams Chat Content Moderation Service – CST8917 Lab 3

## 🧠 Overview
This project implements a real-time Microsoft Teams chat content moderation system using **Azure Logic Apps**. The workflow monitors messages posted to a Teams channel and detects inappropriate language. When violations are found, the system automatically triggers an **email alert** to notify the administrator.

> ✅ This solution demonstrates serverless workflow automation using Logic Apps, and optionally integrates **Azure Functions** and **Azure Cognitive Services for Language** to enhance content analysis.

---

## 🔧 Technologies Used
- **Azure Logic Apps** – to design and run the automated workflow
- **Microsoft Teams** – source of monitored chat messages
- **Outlook (Office 365)** – sends alert emails
- *(Optional)* **Azure Cognitive Services (Language)** – detects offensive content via AI
- *(Optional)* **Azure Functions** – preprocesses or cleans messages before analysis

---

**Workflow Summary:**

```text
Teams Channel Message
        ↓
Logic App Trigger (New message in channel)
        ↓
Condition: Does message contain banned word(s)?
        ↓                    ↓
   Yes → Send Email       No → End

```
## youtube video
https://youtu.be/x9CKselZFm0
