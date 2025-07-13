# 🤖 Telegram PDF Assistant with n8n

A powerful and intelligent Telegram bot powered by **n8n** that allows users to send PDF documents and perform advanced tasks such as:

- 📄 **Summarize** the contents of a PDF
- 🌐 **Translate** the document into another language
- ❓ **Ask questions** about the contents of the document using LLMs (OpenAI)

## 📦 Features

- **Telegram Bot Integration**: Users interact directly via chat.
- **PDF Support**: Handles PDF file uploads from users.
- **Text Extraction**: Uses PDF.co and OCR.space to extract content.
- **Natural Language Processing**: Integrates with OpenAI GPT-4o via LangChain agent nodes.
- **Dynamic Interaction**: Users choose commands like "Summarize", "Translate", or "Ask a question".
- **Google Sheets Logging**: Optionally logs chat history or actions to Google Sheets for later tracking.

## ⚙️ Technologies Used

- [n8n](https://n8n.io)
- [Telegram Bot API](https://core.telegram.org/bots/api)
- [PDF.co](https://pdf.co)
- [OCR.space](https://ocr.space)
- [OpenAI (GPT-4o-mini)](https://openai.com)
- [Google Sheets API](https://developers.google.com/sheets/api)

## 🛠 How It Works

1. **User sends a PDF file** via Telegram.
2. **Bot asks** what to do: Summarize, Translate, or Ask a question.
3. Depending on the choice:
   - The file is downloaded and converted to text.
   - The text is processed by a LangChain Agent using OpenAI.
   - The result is sent back to the user.

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/telegram-pdf-assistant-n8n.git
2. Import My_workflow.json into your n8n instance.

3. Set up the following credentials in n8n:

  - Telegram Bot API.
  - PDF.co API key.
  - OCR.space API key.
  - OpenAI API key.
  - Google Sheets OAuth2 (optional).

4. Deploy and activate the workflow.

## 📂 Folder Structure
.
├── workflows/.
│   └── My_workflow.json  # Main n8n flow.
└── README.md             # This file.

## ✅ Use Cases
Academic research summarization.
Multilingual document processing.
Legal or technical document Q&A.
Lightweight AI assistant for Telegram.

## 📝 License
MIT License
