# n8n-whatsapp-resume-bot
WhatsApp bot built with n8n that collects candidate data and generates a CV.

This repository contains an exported n8n workflow (`whatsapp-resume-bot.json`) that implements a WhatsApp-based resume assistant.

The bot:

- Receives messages from candidates via WhatsApp (WhatsApp Business Cloud API + n8n).
- Asks structured questions and collects all required information for a CV.
- Automatically generates a structured resume (CV) from the provided data.
- Can forward the generated resume to potential employers (for example via email or API integrations).

## Features

- Built with **n8n** (self-hosted or n8n Cloud).
- Integration with **WhatsApp Business Cloud API**.
- Conversation-driven data collection (name, contact details, experience, skills, desired position, etc.).
- Easy to adapt to different languages, industries or resume templates.

## How to use

1. Install and run n8n (Docker, desktop or server).
2. In the n8n UI go to:  
   `Workflows` → `Import from File` → select `whatsapp-resume-bot.json`.
3. Configure your credentials:
   - WhatsApp Business Cloud API (App ID, App Secret, permanent access token, webhook URL).
   - Optional: SMTP or other services for sending the generated CV to employers.
4. Activate the workflow.
5. Connect your WhatsApp webhook in the Meta Developer Console to the n8n webhook URL of this workflow.
6. Send a test message from WhatsApp to start the conversation.

## Disclaimer

This project is a demo/portfolio workflow to showcase how n8n and WhatsApp can be used to automate the recruitment and application process.  
Please make sure to comply with all relevant data protection and privacy regulations (e.g. GDPR) when using it with real candidates.

