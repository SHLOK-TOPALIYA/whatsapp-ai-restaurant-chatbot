<div align="center">

# 🤖 WhatsApp AI Restaurant Chatbot

**An AI-powered WhatsApp assistant that handles restaurant orders, FAQs, and inventory — automatically.**

![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=for-the-badge&logo=google-gemini&logoColor=white)
![WhatsApp](https://img.shields.io/badge/WhatsApp_Business_API-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)

</div>

---

## 📌 Overview

This project automates restaurant customer service directly on WhatsApp. Customers can ask questions, check food availability, and place orders — all through natural conversation — while an **n8n** workflow powered by **Google Gemini** handles the logic and **Google Sheets** acts as the live order/inventory database.

No app to download. No forms to fill. Just a WhatsApp chat.

## ✨ Features

- 🍽️ **AI-powered ordering** — customers order in plain language
- 📋 **FAQ support** — instant answers to common restaurant questions
- 📦 **Real-time inventory checks** — no more "sorry, that's out of stock" after ordering
- 🛒 **Automatic order management** — orders logged without manual entry
- 📱 **Native WhatsApp Business integration**
- 🧠 **Conversation memory** — the bot remembers context mid-chat
- 📊 **Google Sheets backend** — zero-setup database for small restaurants

## 🛠️ Tech Stack

- **Automation:** n8n (workflow engine)
- **AI Model:** Google Gemini API
- **Messaging:** WhatsApp Business Cloud API
- **Storage:** Google Sheets
- **Architecture:** AI Agent + JSON-based workflow

## ⚙️ How It Works

![Workflow Architecture](./workflow.png)

1. **WhatsApp Trigger** — incoming customer message kicks off the workflow
2. **AI Agent** — the central brain that interprets intent and decides what to do next
3. **Google Gemini Chat Model** — powers the AI Agent's language understanding and responses
4. **Simple Memory** — keeps track of conversation context across messages
5. **Get Inventory** *(reads Google Sheet)* — checks live stock before confirming an order
6. **Get FAQ** *(reads Google Sheet)* — pulls answers to common restaurant questions
7. **Post Orders** *(appends to Google Sheet)* — logs new orders automatically
8. **Send Message** — the AI Agent's reply is sent back to the customer on WhatsApp

## 🎥 Demo

A full walkthrough is available in this repo: `chatbot-demo.mp4`

## 📁 Project Files

```
WhatsApp-AI-Chatbot/
├── restaurant-ai-chatbot-workflow.json   # Importable n8n workflow
├── workflow.png                          # Architecture diagram
└── chatbot-demo.mp4                      # Demo video
```

## 🚀 Setup

1. Import `restaurant-ai-chatbot-workflow.json` into your n8n instance
2. Connect your **WhatsApp Business API** credentials
3. Add your **Google Gemini API** key
4. Link a **Google Sheet** for inventory and order tracking
5. Activate the workflow and message your WhatsApp number to test

## 🚀 Roadmap

- [ ] Payment gateway integration
- [ ] Order tracking for customers
- [ ] Live delivery status updates
- [ ] Voice message support
- [ ] Multi-language support

## 👨‍💻 Author

**Shlok Topaliya**
Dhirubhai Ambani University (formerly DA-IICT)

---

<div align="center">
⭐ Found this useful? Star the repo and share it with a restaurant owner!
</div>
