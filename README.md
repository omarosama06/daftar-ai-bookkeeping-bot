# Daftar – AI Bookkeeping Bot for Telegram (n8n)

Daftar is an n8n workflow that lets small business owners in Egypt
manage their expenses through a Telegram chat. Users send a photo of
a receipt, a voice note, or a short text message, and the bot records
it in a ledger. Messages are in Arabic.

## Features
- **Receipt scanning:** an AI vision model reads receipt and invoice
  images (Arabic and English) and extracts vendor, amount and category
- **Voice notes:** voice messages are transcribed and logged as expenses
- **Text input:** write an expense in plain language, or ask a question
  about your spending
- **Confirmation step:** the bot asks the user to approve an entry
  before it is saved
- **Undo:** delete the last recorded entry
- **Weekly report:** a scheduled AI summary of spending sent on Telegram
- **Receipt storage:** receipt images are saved to Google Drive

## Tools used
n8n, Telegram Bot API, OpenAI (GPT-4o-mini, transcription,
embeddings), Qdrant vector store, Google Sheets, Google Drive

## How to run it
1. Import `daftar-workflow.json` in n8n (Workflows → Import from file)
2. Create your own credentials: Telegram bot, OpenAI, Google Sheets,
   Google Drive, Qdrant
3. Replace the placeholders: `YOUR_GOOGLE_SHEET_ID`,
   `YOUR_DRIVE_FOLDER_ID`, `YOUR_TELEGRAM_CHAT_ID`
4. Create a Google Sheet to use as the ledger
5. Activate the workflow and message your bot

## Screenshot
<img width="1311" height="582" alt="Daftar " src="https://github.com/user-attachments/assets/2a3b6ec8-4d38-4ca8-b329-d60e18d31a5e" />

