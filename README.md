# Email Assistant Workflow (n8n)

This project is a no-code/low-code automation built in [n8n](https://n8n.io/) that:

- Fetches unread emails from Gmail every 15 minutes.
- Extracts subject, body, and sender.
- Sends data to the Gemini API (via Google PaLM/Gemini endpoint) for:
  - Email summarization
  - Category prediction (Work, Personal, Spam, Other)
  - Reply drafting
- Creates a Gmail draft response.
- Labels the email automatically based on the detected category.

## Tools Used
- **n8n**
- **Gmail API**
- **Google Gemini (PaLM) API**

## How to Use
1. Import `workflow.json` into your n8n instance.
2. Add Gmail credentials (OAuth2).
3. Replace the Gemini API key with your own.
4. Activate the workflow.

## Demo Use Case
An intelligent assistant that replies to and organizes emails automatically for professionals, saving time and improving productivity.

