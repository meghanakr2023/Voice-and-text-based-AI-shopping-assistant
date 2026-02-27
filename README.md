🛍️ Voice & Text Based AI Shopping Assistant (n8n + Telegram)

An intelligent Telegram bot built using n8n, capable of understanding both voice and text messages to provide:

🛒 Product search from Amazon India

👗 Personalized styling advice

🎤 Voice-to-text conversion using AI

🤖 Conversational shopping assistant

🚀 Features
🛒 Product Search

User asks: "Puma shoes under 5000"

Bot searches Amazon India

Returns top product results with:

Product name

Price

Rating

Product link

👗 Styling Assistant

User asks: "How to style blue jeans?"

Bot asks clarifying questions

Provides personalized outfit suggestions

🎤 Voice Support

Accepts Telegram voice messages

Converts speech → text using AI (Whisper via Groq)

Processes the request like normal text

🧠 How It Works (Workflow)
📩 Input Handling

Telegram Trigger receives:

Text messages

Voice messages

If voice message detected:

Download audio file

Convert .oga → .ogg

Send to speech-to-text API

Get transcription

🤖 AI Processing

Uses Google Gemini Chat Model with custom system prompt:

Determines intent (product search or styling)

Calls tools when needed

Generates response

🌐 Product Scraping Tool

Scrapes Amazon India search results using Scraper API.

🧩 n8n Workflow Architecture
Telegram → Detect Voice/Text → Transcribe (if voice)
       → AI Agent → (Optional Tool Call)
       → Send Reply to Telegram
🛠️ Technologies Used

n8n — Workflow automation

Telegram Bot API

Google Gemini AI

Groq Whisper (Speech-to-Text)

Scraper API — Amazon scraping

⚙️ Setup Instructions
Prerequisites

n8n installed

Telegram Bot Token

Google Gemini API Key

Groq API Key

Scraper API Key

Import Workflow

Download the JSON workflow file

Open n8n

Import workflow

Configure credentials

Configure Credentials

Add in n8n:

Telegram credentials

Gemini API credentials

Groq API key

Scraper API key

⚠️ Do NOT upload secrets to GitHub

💬 Example Commands

Product Search

Show me running shoes under 3000

Styling Advice

Outfit ideas for wedding

Voice Input
Send a voice message 🎤

📌 Use Cases

AI shopping assistant

Fashion advisor bot

Voice-enabled chatbots

Conversational commerce

👩‍💻 Author

Meghana K R
B.E. Computer Science & Design
AI & Web Development Enthusiast 🚀
