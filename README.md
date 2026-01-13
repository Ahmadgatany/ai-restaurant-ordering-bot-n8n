# AI Restaurant Ordering Bot (n8n)

An end-to-end AI-powered restaurant ordering chatbot built using **n8n**, **LLMs**, **Telegram**, and **Google Sheets**.

This project demonstrates how to design a reliable, stateful conversational system using no-code / low-code automation combined with large language models.

---

## 🚀 Features

- Telegram-based chatbot interface
- Automatic customer identification using Telegram ID
- Customer data collection (name & phone number)
- Menu presentation on demand
- Order extraction from natural language (Arabic)
- Order confirmation flow (no infinite loops)
- Structured AI outputs for safe automation
- Orders stored in Google Sheets

---

## 🧠 Architecture Overview

The workflow is designed as a multi-stage pipeline:

1. **Telegram Trigger**
   - Receives incoming user messages.

2. **Customer Lookup (Google Sheets)**
   - Checks if the Telegram ID already exists.

3. **Customer Info Collection (LLM)**
   - Collects name and phone number for new users only.
   - Prevents repeated data requests.

4. **Menu & Order Handling (LLM)**
   - Shows menu on request.
   - Extracts selected dish, price, and sandwich flag.
   - Confirms the order before final submission.

5. **Order Storage**
   - Saves confirmed orders into Google Sheets.

6. **Telegram Response**
   - Sends user-friendly confirmations and prompts.

---

## 🧩 Technologies Used

- **n8n** – Workflow automation
- **OpenRouter (LLMs)** – Natural language understanding
- **Telegram Bot API** – User interaction
- **Google Sheets** – Lightweight database
- **Structured Output Parsing** – Reliable AI-to-automation bridge

---

## 📂 Files

- `AI Bot Orders.json`  
  Exported n8n workflow (no credentials included).

- `assets/workflow.png`  
  Visual overview of the workflow (optional).

---

## 🔐 Security Notes

- No API keys or credentials are included in this repository.
- All secrets (Telegram token, OpenRouter API key, Google credentials) are managed securely via n8n Credentials.

---

## 🧪 Use Case

This project was built as a practical task during an **n8n automation course**, and extended into a **production-ready AI ordering system** to demonstrate real-world automation patterns.

---

## 📌 Author

Built by **Ahmed Gaitani**  
AI / Automation Engineer

---

## 📎 Preview

> A visual representation of the workflow is included to show the full logic and routing.
