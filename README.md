# 🛍️ Voice & Text-Based AI Shopping Assistant — n8n Workflow

An AI-powered shopping and styling assistant built using n8n that interacts with users on Telegram through both voice and text messages.

The assistant can search products from Amazon India and provide personalized styling advice.

---

## 🚀 Features

🎤 Accepts voice messages and converts them to text
💬 Supports text-based conversations
🛒 Searches products from Amazon India
👗 Provides personalized styling advice
🤖 AI-powered conversational assistant
📱 Telegram bot integration

---

## 🧠 How It Works

### 🔹 Voice Mode

1. User sends a voice message on Telegram
2. Audio is downloaded and processed
3. Speech is converted to text using AI
4. AI assistant processes the request

---

### 🔹 Text Mode

1. User sends a text message
2. AI assistant understands the intent
3. Responds with product results or styling tips

---

### 🛍️ Product Search Mode

When users ask for products (e.g., "running shoes under ₹3000"):

* Builds Amazon India search URL
* Scrapes product data using Scraper API
* Extracts product name, price, rating, and link
* Shows top results to the user

---

### 👗 Styling Assistant Mode

When users ask fashion-related questions:

* Asks clarifying questions (occasion, style, color, etc.)
* Provides personalized outfit suggestions
* Recommends accessories and styling tips
* Offers to search products if needed

---

## 🛠️ Tools & Integrations Used

* **n8n** — Workflow automation
* **Telegram Bot API** — User interaction
* **Google Gemini AI** — Conversational intelligence
* **Groq Whisper API** — Speech-to-text conversion
* **Scraper API** — Product data extraction
* **Amazon India** — Product search source

---

## 📌 Workflow Components

* Telegram Trigger (receives messages)
* Voice detection and processing
* Speech-to-text conversion
* AI Agent for conversation
* Product scraping tool
* Response delivery via Telegram

---

## 📂 Files

* `workflow.json` — Exported n8n workflow file

---

## ⭐ Example Use Cases

### 🎤 Voice Input

"Show me white sneakers under 3000"

### 💬 Text Input

"How to style a blue kurti for a wedding?"

### Output

✔ Product recommendations
✔ Styling suggestions
✔ Interactive conversation

---

## ⚙️ How to Use

1. Import `workflow.json` into n8n
2. Configure Telegram Bot credentials
3. Configure AI and API credentials
4. Activate the workflow
5. Start chatting with the bot

---

## 🎯 Purpose

This project demonstrates an AI-driven conversational assistant capable of:

* Voice and text interaction
* E-commerce product search
* Personalized recommendations
* Multi-service integration

---

## 👩‍💻 Developed By

**Meghana K R**
B.E Computer Science & Design
Mysore University

---

## 📜 License

For educational and demonstration purposes.

---
